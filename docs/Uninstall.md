## Uninstalling the CLI

  Windows (Command Prompt/PowerShell)


   1. Open Command Prompt or PowerShell.
   2. Navigate to the directory where you cloned the repository. (e.g., cd C:\Users\Admin)
   3. Unlink the npm package (if you linked it):


   1     npm unlink gemini-cli-sidx1fork

      Explanation: This command removes the global symbolic link created by `npm link`, if it exists. It
  might show an error if it wasn't linked or the link is already gone, which is fine.
   4. Remove the project directory:

   1     rmdir /s /q gemini-cli-sidx1fork

      Explanation: `rmdir` is the command to remove directories. `/s` removes all subdirectories and files.
  `/q` performs the removal quietly, without asking for confirmation.


  macOS and Linux (Bash/Zsh)


   1. Open your Terminal.
   2. Navigate to the directory where you cloned the repository. (e.g., cd /home/youruser/ or cd
      /Users/youruser/)
   3. Unlink the npm package (if you linked it):

   1     npm unlink gemini-cli-sidx1fork

      Explanation: This command removes the global symbolic link created by `npm link`, if it exists. It
  might show an error if it wasn't linked or the link is already gone, which is fine.
   4. Remove the project directory:

   1     rm -rf gemini-cli-sidx1fork

      Explanation: `rm` is the command to remove files and directories. `-r` (recursive) allows it to remove
   directories and their contents. `-f` (force) makes it remove files without prompting for confirmation.
