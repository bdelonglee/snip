#### SYSTEM Find X OR Y basic
find . \( -iname "*.exr" -o -iname "*.jpeg" \)


#### SYSTEM Find X OR Y Sub options
find /media/d/ -type f -size +50M ! \( -name "*deb" -o -name "*vmdk" \)


#### SYSTEM Find x or y AND s or t
find . \( -name "*.bash" -o -name "*.txt" \) \( -mtime +180 -o -mtime -10 \) -size +2K -exec ls -ltr {} \;


#### SYSTEM Find Exec
find . -name "*.bash" -mtime +180 -size +2K -exec ls -l {} \;


#### SYSTEM Find Exec Qts
find . -iname "*mov" -exec rv-xenvi {} +


#### SYSTEM Find NOT
find . -type f ! -name "*.txt" -mtime -30 -exec ls -l {} \;


#### SYSTEM Number of files in current directory
ls -1 | wc -l


#### SYSTEM Find Delete, lorsque argument list is too long avec RM
find . -name "*.pdf" -delete


#### SYSTEM Print Python path
python -c "import sys; print(':'.join(x for x in sys.path if x))"



#### SYSTEM MacOs Drag Windows
defaults write -g NSWindowShouldDragOnGesture -bool true  
defaults delete -g NSWindowShouldDragOnGesture


#### SYSTEM Linux Mate panel
mate-panel --reset


#### SYSTEM Rsync Mac to Box
rsync  -av --exclude="*.svg" ~/Documents/PROJECTS/DEV/ivy bdelonglee@box207:/u/hqr/FILM/WORK/SUP_SHELL_SCRIPTS/prod/


#### SYSTEM Rsync Box to Mac 
rsync  -av --exclude="*.svg" bdelonglee@box207:/u/hqr/FILM/WORK/SUP_SHELL_SCRIPTS/prod/ ~/Documents/PROJECTS/DEV/ivy 


#### SYSTEM Scp
scp  -rv ~/Documents/PROJECTS/DEV/ivy bdelonglee@box207:/u/hqr/FILM/WORK/SUP_SHELL_SCRIPTS/prod/


#### SYSTEM Tree Exclude
tree -C -I '*.svg|*.png'


#### SYSTEM Tree List Only
tree -C -P '*.py|*.css'


#### SYSTEM File count Size recursive
find . -type f | wc -l


#### SYSTEM File count Size recursive (no hidden file or directory)
find . -not -path '*/[@.]*' -type f | wc -l


#### SYSTEM Find Fullpath Full FZF
find "$PWD" | fzf | pbcopy


#### SYSTEM Find Fullpath Full
find "$PWD"


#### SYSTEM Find Fullpath Full  Bat
find "$PWD" | bat


#### SYSTEM Find Fullpath Relative
find . 
