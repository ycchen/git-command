#### Git log
$ git log <path to the file>

#### Git diff file across branches
$ git diff branchA branchB <path to the file>

#### How to get diff on a file between commit
$ git diff <commit number>:<path to a file> <commit number>:<path to a file>

$ git diff 69140f2:lib/data_row_validator.rb fcb4ca8:lib/data_row_validator.rb

$ git diff 5cc287:pom.xml e8e420:pom.xml

$ git diff 3aa914:pom.xml 7476e1:pom.xml

$ git diff 422bfd:pom.xml f92ad8:pom.xml

#### To see all changes to the file between 2 commits on commit-by-commit basis
$ git log -u 69140f2..fcb4ca8 -- lib/data_row_validator.rb

#### Stash
$ git stash list

$ git stash pop # apply stash <revision> then remove the stash

$ git stash

#### Get a file from a specific commit
$ git show <commit version>:<path to the file> 

$ git show a7ba6e4:app/controllers/application_controller.rb

#### get diff between local and remote
$ git diff origin/<branch name>

$ git diff origin/collect4

$ git diff origin/master

#### Search within git log command

/ <commit number>

http://stackoverflow.com/questions/7124914/how-to-search-a-git-repository-by-commit-message

#### Get all change from log
$ git log -p

#### Search commit log
$ git log --all --grep='Buid 0051'

#### If you seem to have lost your history, check the 'reflog' as your safety net
$ git reflog
