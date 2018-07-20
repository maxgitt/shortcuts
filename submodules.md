## Adding a submodule
cd my_workspace/
git submodule add [URL]

## Removing a submodule
git submodule deinit [submodule/path]
git rm submodule/path
git status

## Cloning the entire workspace
git clone --recursive-submodules [URL]
OR
git clone [URL]
cd workspace/
git submodule update --init --recursive // recursively init all submodule repos

## Checking status
git submodule status
(+) sign means workspace is pointing to different submodule commit // i.e. submodule is behind

## Git log
git log --oneline --decorate

## Updating
git submodule update
git submodule update --checkout?
cd [submodule/path]
git pull

## Working in a Submodule
**Ensure you are on a working branch**

