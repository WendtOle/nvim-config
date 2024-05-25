# basic setup
used youtube tutorial: https://www.youtube.com/watch?v=CVCBHHFXWNE
remove current .config/nvim folder
clear cached stuff
clone with command git clone -b v2.0 https://github.com/NvChad/NvChad ~/.config/nvim --depth 1
start nvim with "nvim"
should install dependencies as shown in the tutorial

# install typescript language server
- link plugins.lua from chadrc.lua
- add entry in plugins.lua which uses Mason (dependency manager) to ensure that typescript language server is installed
- close nvim (:qa!) and reopen it
- run command ":MasonInstallAll" to actually install language server by Mason

