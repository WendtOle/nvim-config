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
- we then use the nvim-lspconfig plugin and overwrite some configurations
- we use the NnChad configuration file "plugins.configs.lspconfig" and add a custom one -> custom/configs/lspconfig.lua 
- in the custom lspconfig file we pull out on_attach and capabilities from the NvChad configuration
- then the lspconfig package is imported 
- then comes a block which i do not complelety understand 
- its about binding the tsserver stuff to the lspconfig attributes
- then we adjust the initial options of the typescript language server
