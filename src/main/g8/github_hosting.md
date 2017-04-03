# GitHub Hosting Documentation

Before hosting the project on GitHub, ensure that the code has been cleared, and released for open source.
1.	Go to github.com/jpl-imce and sign in
2.	Click on “New” button, or visit https://github.com/organizations/JPL-IMCE/repositories/new
3. Enter a repository name which matches the project name (beginning with gov.nasa.jpl…)
      1. Enter a short description of the project. Focus this description on the main functionality of the component
      2. Choose “Public” as repository type, leave the rest as default
      3. Click “Create Repository”
3.	Set remote / origin locally, do initial commit

## GPG

You must configure a persistent GPG agent to run in order to GPG sign commits. This is required for our work, as we must have a continuous history of GPG-signed commits in order to meet open-source standards. Furthermore, it is good practice in enforcing traceability and accountability on the part of developers. Your signature is a way of guaranteeing that it is you who made the commit, and that you stand behind the code you have written.

See the [GPG guide](gpg.md) for instructions.


## "GitS" for automatic GPG signing of Git commits

Git has GPG signing capabilities built-in, which allow for developers to "sign" a commit and therefore ensure the legitimacy of the code it contains. This capability is typically utilized by providing command line arguments to Git operations like commits or merges (see the [Git documentation](https://git-scm.com/book/en/v2/Git-Tools-Signing-Your-Work) for more information).

We have produced our own script `gitS` that you can call when performing Git operations, and it will take care of adding the signing arguments when appropriate. **Note:** this scripts assumes your Git executable is at `/usr/bin/git`, because this is the location on the Virtual Machine. You may need to edit the script if Git is in a different location on your computer.

Download [`gitS`](scripts/gitS) and place it in a permanent location (ie. `/usr/local/bin`). I recommend you make an alias such that you can call this script directly from the command line in the same way that you would call Git normally. If you don't want it to mask you default executable, then alias it to `gits` by adding the following line to your `~/.bash_profile`:
```
alias gits='/path/to/gitS'
```

This way, whenever you type `gits` at the command line, the script will be used, but you can always use `git` as normal for other work.




