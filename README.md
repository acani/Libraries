# Libraries

Instructions on how to add a Git repository (named `RepositoryName`) to your Xcode project

1. Download

    From the root directory of your project's main Git repository, run:

        git submodule add git://github.com/acani/RepositoryName.git Libraries/RepositoryName

2. Install

    From Finder, drag the newly created directory to your project's project navigator in Xcode.

    Uncheck "Copy items if needed," select "Create groups," and uncheck all targets.

    In Xcode, remove the reference to `RepositoryName/.gitignore`.

    Add the Swift files (pattern: `RepositoryName/*.swift`) to your target.

3. Use

    See `RepositoryName/README.md` for usage information.

4. Update

    Run `git pull` from `Libraries/RepositoryName`.
    
    If that adds, moves, or removes any files, update your Xcode project accordingly.
