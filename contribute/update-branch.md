# Keep Branch Up-To-Date

It's a good idea to push your local changes to the repo on a regular basis.  Complete the following procedure to do so.

## [Optional] View Pending Changes

It's usually helpful before you push changes to see what they are first.  Complete the following steps to see the changes you haven't pushed yet.

1.  Open a [svcmtctest1](https://github.com/MichelBarnett/svcmtctest1) command prompt

2. Execute the following:

   ```powershell
   git status
   ```

   Here's an example of what you'll see:

   ![]()

## Push Changes

1.  Open a [svcmtctest1](https://github.com/MichelBarnett/svcmtctest1) command prompt

2. Stage your changes by using the `git add` command. For example:

   ```
   git add .
   ```

   > [!NOTE]
   >
   > We're specifying `.` as an argument to `git add` which means: *stage all new, modified, deleted files in the current directory and all sub-directories*.  There are many variations on this.  See documentation on the [git add](https://github.com/git-guides/git-add) command for more detail.

3. Create a commit

   ```
   git commit -m "<YourComment>"
   
   ```

   for example:

   ```powershell
   git commit -m "added introduction to troubleshooting guide"
   ```

   > [!TIP]
   >
   > Make your comment descriptive so it's easier to identify the associated changes.

4. Push your changes by executing:

   ```powershell
   git push
   ```

Now your local changes are synced with the github repo.