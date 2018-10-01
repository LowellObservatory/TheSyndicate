# Code Standards

These are the things that must be settled/cleared before code is considered
acceptable.  It will likely be a flexible and sliding set of requirements
rather than a draconian/rigid framework, though some of it could be
implimented as automated checks from a CI system for every pull request.

- PEP-8 conformity, as checked and verified by the agreed-upon pylintrc file.
    - Spaces instead of tabs, in blocks of 4
    - See also this [sample pylintrc](pylintrc)
- Codes designed for command-line use shall not just dump everything into
  the ```__main__``` function but rather a distinct ```main()``` function
  or similar that is called from ```__main__```.  This is to ensure that
  pylint (or other linters) can check for unused variables and we always have
  control over global scope variables.

## Continious Integration (CI) Testing

Q: Do we want to try to get this in place?  It likely has a low/moderate setup
   cost in terms of time (1-2 days?) but would automate the checking of
   the codebases for the basics mentioned above.
   
   Examples:
   
   - [CircleCI](https://github.com/marketplace/circleci)
   
   - [TravisCI](https://github.com/marketplace/travis-ci)
   
   - [Hound](https://github.com/marketplace/hound)

   I'll just add that LSST is using TravisCI for most things, and might
   be a good starting point to see if it'll work for us.
   
   Michael Mommert's AstroPy GitHub group is using Travis-CI as well so
   it seems like it would be the best choice for us.

# Documentation Tools to Use

- PyDoc
- sphinx
- ?

# Code Review Tools

- [Review Ninja](https://github.com/reviewninja/review.ninja)
