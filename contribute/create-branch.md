# Create Branch

In order to contribute changes to the repo, you'll need to create a branch to store your work before it's merged.  Complete the following procedures to do so.

## Create a Branch

1. Open a [svcmtctest1](https://github.com/MichelBarnett/svcmtctest1)command prompt.

2. Create a branch by executing the following:

   ```powershell
   git checkout -b <UserName>/<BranchName> 
   ```

   for example:

   ```powershell
   git checkout -b MichelBarnett/alternator
   ```

   > [!NOTE]
   >
   > By convention prefix the branch with your user name and a forward slash and then choose a branch name that reflects the work you're doing.  In this example, we're creating a branch for a new alternator troubleshooting guide.

## Associate the Local and Remote Branch

Before we can push changes we need to associate the local branch we just created with a corresponding branch in the GitHub repo.  Complete the following procedure to do so.

1. In the same command prompt execute:

   ```powershell
   git push
   ```

   The response will look something like this:

   ```powershell
   fatal: The current branch michelbarnett/contributeaboutupdate has no upstream branch.
   To push the current branch and set the remote as upstream, use
   
       git push --set-upstream origin michelbarnett/contributeaboutupdate
   ```

   > [!NOTE]
   >
   > This command is what we want.  Running `git push` when we know it'll fail is an easy way to get git to generate the command for us.

2. Execute the following command:

   ```powershell
   git push --set-upstream origin michelbarnett/contributeaboutupdate
   ```

   This associates our local branch with a remote branch in the repo (that's named the same).  From now on you can push changes simply by executing `git push`.  

