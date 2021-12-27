# hashicorp-packer
Repository for HashiCorp Packer course.

**Install Vim configs:**

    curl https://raw.githubusercontent.com/smart-cn/hashicorp-packer/master/env/vimrc -o ~/.vimrc
**Update(Install) Vim to v8.x on Centos 7 from sources:**

    mkdir vim-src && cd vim-src/

    git clone https://github.com/vim/vim.git .

    yum install gcc make ncurses ncurses-devel

    sudo yum install ctags git tcl-devel \
    ruby ruby-devel \
    lua lua-devel \
    luajit luajit-devel \
    python python-devel \
    perl perl-devel \
    perl-ExtUtils-ParseXS \
    perl-ExtUtils-XSpp \
    perl-ExtUtils-CBuilder \
    perl-ExtUtils-Embed

    sudo ./configure --with-features=huge \
    --enable-multibyte \
    --enable-rubyinterp \
    --enable-pythoninterp \
    --enable-perlinterp \
    --enable-luainterp

    sudo make

    sudo yum remove vim-enhanced vim-common vim-filesystem

    sudo install
**Install HashiCorp HCL plugin for Vim:**
```
mkdir -p ~/.vim/pack/jvirtanen/start

cd ~/.vim/pack/jvirtanen/start

git clone git://github.com/jvirtanen/vim-hcl.git
```
