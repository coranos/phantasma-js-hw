### to force only one version of phantasma-js-hw

  rm -rf .git;
  git init;
  git checkout -b main;
  find . -exec touch {} \;
  git add .;
  git commit -m "Initial commit";
  git remote add origin https://github.com/coranos/phantasma-js-hw.git;
  git push -u --force origin main;
  git branch --set-upstream-to=origin/main main;
  git pull;git push;

## to force local version to match origin/master

  git fetch --all;
  git reset --hard origin/master;
