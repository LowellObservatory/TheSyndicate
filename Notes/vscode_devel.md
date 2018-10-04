0. Clone the initial repository.
    - In vscode, hit 'F1' or View -> Command Palette
        - Type 'git clone' and hit enter. It'll prompt you for the
          remote repository URL, so copy and paste in a github URL
          (e.g. https://github.com/LowellObservatory/ArcCon) and hit enter.
          It'll then prompt you for a local place on your computer where you
          want the repository to go; it will be a subdirectory of whatever
          directory you choose, with the name the same as the repository.
        - After it's done, it'll prompt you in the bottom whether you want
          to open the repository or not. Open it up!
1. Make a new branch of the repository, Ryan might call his RyansBranch.
    - Get back to that command palette from above and type 'git create branch'
      and hit enter.
2. Develop! Make changes, do whatever. Make a few commits.
    - On your first commit, make sure you push the changes to github.
    - It'll notice that the branch isn't on github yet, and ask you
      something like:
          "The branch 'RyansBranch' has no upstream branch.
           Would you like to publish this branch?"
      The answer is 'OK' to actually do it.
    - Keep making commits, and when you're done (or when you want) push them
      to github.
          - Making the new branch automatically put your local repository
            onto the new branch.  If you ever need to jump between branches,
            the Command Palette is your friend.
              - NOTE: You can't have any unsaved changes to files and switch
                branches.  Those changes must be committed, discarded, or
                stashed before you can go to another branch! This is true
                for git in general, and some IDEs or git clients will
                stash stuff automagically for you.