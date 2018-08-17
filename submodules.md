## Adding a submodule
cd my_workspace/  
git submodule add [URL]

## Removing a submodule
git submodule deinit [submodule/path]  
git rm submodule/path  
git status  

## Cloning the entire workspace
git clone --recursive [URL]  
  
OR  
  
git clone [URL]  
cd workspace/  
git submodule update --init --recursive // recursively init all submodule repos  

## (won't update submodules if parent wasn't changed, look into tracking branch)
git submodule status  
(+) sign means workspace is pointing to different submodule commit // i.e. submodule is behind  

## Git log
git log --oneline --decorate  

## Updating your submodules
git submodule update (will put you in a headless state)
cd [submodule/path]  
cd checkout [branch name]
git pull  
  
OR  
  
git submodule foreach git pull origin master  

## Working in a Submodule
**Ensure you are on a working branch**

