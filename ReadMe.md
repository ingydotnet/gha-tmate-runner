gha-tmate-runner
================

Start a tmate session inside a GitHub Actions runner.


# Usage

Something like this:

* Modify the config
* `git commit -a --amend --no-edit && git push`
* Go to https://github.com/ingydotnet/gha-tmate-runner/actions
  * Open the log view
  * Wait for the `ssh` command to print
  * eg: `ssh YKa7ukZedkEJ3Gg4n3CHnaGzp@sfo2.tmate.io`
  * Copy the command
* Paste and run the command in a terminal
* Now I'm shelled into the GHA container/VM
* Play around
* Exit the shell
* The GHA session ends

Sometimes the session becomes broken while using it; especially when using the
Windows CMD shell.
If this happens, click the "Cancel workflow" button in the GHA web page.

Remember you only get so many minutes a month to use GHA for free, so be
mindful not to leave the tmate running.
