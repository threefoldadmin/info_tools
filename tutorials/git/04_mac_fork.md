# GIT on Mac OS with Fork application

## Preface
Git is a command-line tool. Therefore when you will search in internet, you will find most of the manuals talking about commands, not buttons or actions.

However there are plenty of friendly and free user-interface tools for any system.

We will show how to use [Fork](https://git-fork.com) for Mac OS X.

## 0. Installation

1. Go to [https://git-fork.com](https://git-fork.com) and download it.
![Download fork](https://docs.greenitglobe.com/company30/tutorials_basic/raw/master/git/images/fork_download.png)
2. Install application
3. Start Fork application and enter your login and email:
![Authorize](images/fork_authorization.png)

## 1. Starting work with new repository (Clone command)
1. Open GOGs (remote repository that you need to start work with).
2. Click `SSH` Button on the right side and copy link in the text box:
![SSH](images/gogs_clone_repo.png)
3. Open fork and click `Add Repository` -> `Clone`:
![Clone repo](images/fork_clone_button.png)
4. Paste link to the remote repo from the step 2 to the `Repository URL` field and click `Clone` button:
![Clone dialog](images/fork_clone_dialog.png)
5. Repository is ready for work, you will see tree of recent changes on the main window:
![New repo dialog](images/fork_new_repo.png)
6. You can navigate to the folder where your local repository is located by clicking the `Navigate` (icon with up arrow) menu -> `Show in Finder` button:
![Show in finder](images/fork_show_in_finder.png)

## 2. Staring new work session (Pull command)
Every time you want to start work with documents you have to get latest updates from remote server.
If you skip these step you will have high chances to face issues when you will try to save changes after your work, especially if somebody else did any changes in the files you are going to edit. Doing this simple steps will ensure you work on the latest version of the repository.
1. In order to do this, you have to click "Pull" button:
![Pull button](images/fork_pull_button.png)
2. You will see following dialog, press `Pull` button:
![Pull dialog](images/fork_pull_dialog.png)
3. In case no error messages are shown, you can freely start your work.

## 3. Save changes (Commit and Push commands)
1. Stage changes. By doing this you will ask git to take a look at your changes and index them.
 * Go to changes section:
 ![Change view](images/fork_changes_view.png)
 * Select all changes you have made and click `Stage` button:
 ![Changes selected](images/fork_changes_selected.png)
2. Write short description of changes (and long if needed in the space below) and click `Commit` button.
![Commit dialog](images/fork_commit_dialog.png)
Now your changes are saved and tracked in your local copy of repository.
3. Get (`Pull` button) latest updates from main repository. Check #2 section to see how to do this.
If there is no conflicting changes on the main repository, it will go well. If there is any conflicting changes on the main repository you will be asked to do `Merge` operation. If so, please see the following section (#4 Merge changes)
4. Push changes to the server. To do this, click 'Push' button and then again `Push` on a popped up dialog:
![Push](images/fork_push.png)

## 4. Merge remote and local changes
In case your local changes could not be automatically merged with remote changes you will be asked to merge manually.

1. If automatic merge failed you will see following screen:
![Automerge failed](images/fork_automerge_failed.png)
2. After you close popup, in a stage area you will see a list of files that require merging marked with a Attention sign. Open the one of the files.
3. You will be proposed to merge line by line or choose only one of the versions:
![Merge manually](images/fork_merge_manually.png)
![Choose local](images/fork_merge_choose_local.png)
![Choose remote](images/fork_merge_choose_remote.png)
4. In case you choose to leave only one set of changes, you will have to make ANY edit to the repository and then you will be able to commit once more. If everything is good, next you have to pull again from remote repository and then you can push your merged changes to the server.

* If you choose to merge line by line (both sides checked on the merge dialog), you will see a tool to do it:
![Merge tool](images/fork_merge_tool.png)

In this tool you can merge changes line by line. When you finish merging, just close the window and save changes to the file.

* You also can merge fully manually editing file itself (if it is in text format). Changes from different versions separated by `<<<<<<<<`, `========` and `>>>>>>>` separators:
![Merge manually](images/atom_unmerged_file.png)

* As soon as you finish merging files, you have to do a commit (#3 section), then pull and push commands.

## 5. Final words

Please remember that GIT initially is a command line tool. Therefore sometimes you can get some hard-to-understand error messages if you mess up with something. If you feel that you 'broken' your copy of repository, for you as a beginner, the most easy option could be just to delete the repository folder and clone it again (#1 section - Clone command). In this case you will loose all your local chances unless you do not copy the files somewhere else for your further reference.
If you are are ready to learn more about GIT, how it works and how you can use it like a BOSS, feel free to start running commands in terminal, check official manual, and google all your questions.
