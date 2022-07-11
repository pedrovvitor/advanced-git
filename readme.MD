With git flow installed
Run git flow init and make initial configuration

git flow feature start [branchName]
-> develope your files
git add .
git commit -m 'Add [changesDescription]'
git flow feature finish [branchName]

git flow release start [branchName]
-> develope your files
git add .
git commit -m 'Add [changesDescription]'
git flow feature finish [branchName]