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
3. If you're happy with the branch and think there's good stuff in there,
   head on over to github and create a pull request from your new branch.
   If the repository overlords agree that it's good, and it passes whatever
   checks we agree upon, it'll be merged in.
4. After it's merged in, head back to vscode and pull down the new changes.
   This will update your local copy of the master branch, and the
   process can repeat.