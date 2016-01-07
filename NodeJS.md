# Node.js安装指南

##安裝 NVM （Node Version Manager）

**1. 使用 brew 安裝 NVM**

    brew install nvm

**2. 将下列指令加入.bash_profile（或 .bashrc）档案**

    export NVM_DIR=~/.nvm
    source $(brew --prefix nvm)/nvm.sh

**3. 重新载入 .bash_profile 设定**
    
    source .bash_profile

**4. 测试 nvm 指令**

    MBP:~$ nvm

*注:删除或卸载nvm只需要删除 

    ~/.nvm 
    ~/.npm
    ~/.bower folders*
<br />

##使用 NVM 安裝 Node.js

**1. 找出可安裝的 Node.js 版本**
    
    nvm ls-remote

**2. 安裝 Node.js (0.11.16)**
    
    nvm install 0.11.16

**3. 指定nvm使用的 Node.js版本**
    
    nvm use 0.11.16

**4. 预设使用 0.11.16 版本，否则每次重新链接登入，需要重新nvm use一次**
    
    nvm alias default 0.11.16

**5. 列出所有安裝的版本**

    nvm ls

    *->  v0.11.16<br />
    default -> 0.11.16 (-> v0.11.16)<br />
    unstable -> 0.11 (-> v0.11.16) (default)*

**6. 测试Node.js**

    node -v

    *->  v0.11.16*

**7. 测试 npm**

    npm -v

    *->  2.3.0*

