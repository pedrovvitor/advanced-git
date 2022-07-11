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


Digital Signature for commits

gpg --list-secret-key --keyid-form LONG (list all generated keys)
gpg --full-generate-key

gpg --armor --export[generatedKey]

git config --global user.signingkey [generatedKey]

`Add 'export GPG_TTY=$(tty)' to vim ~/.bash_profile`

git config --global commit.gpgsign true
git config --global tag.gpgsign true