##### Installation

## Step 1 - Install and configure ZSH
---

- Install zsh
    ```
    sudo apt-get install
    ```

- After the installation, change the default shell of the root user to zsh with the chsh command below.
    ```
    chsh -s /usr/bin/zsh root | chsh -s /bin/zsh
```
    
- Check the current shell, /usr/bin/zsh
    ```
    echo $SHELL
    ```

- Revert back to the default shell
    ```
    chsh -s /bin/bash
    ```

## Step 2 - Install and configure Oh-my-zsh framework
---

- Install wget and **git** on the system
    ```
    sudo apt-get install wget
    ```

- Download the installer script and execute it
    ```
    wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh
    ```

- create a new configuration for zsh in root directory
    ```
    ~/.zshrc
    ```

## Step 3 - Install Antigen and configure ~/.zshrc

- Install 
    ```
    curl -L git.io/antigen > antigen.zsh
    ```

- Add the script Antigen script


- After adding the script, reload the .zshrc
    ```
    source ~/.zshrc
    ```
- It automatically install the all the bundles

## Additional plugin configuration
- ### Install Directory Color
    ## Usage
    ---
    This plugin offers two commands:
    - ```lssolarized``` which lists the available solarized themes. For now there are:      
        - ```dircolors.ansi-universal``` (universal theme for 16- and 256-color terminals)
        - ```dircolors.ansi-dark``` (optimized version of universal for dark background)
        - ```dircolors.ansi-light``` (optimized version of universal for light background)
        - ```dircolors.256dark``` (degraded solarized dark theme)
    - ```setupsolarized``` which installs a theme and saves the current configuration to the configuration file (```$HOME/.zsh-dircolors.config``` by default). Without any argument, ```setupsolarized``` will use the theme ```dircolors.ansi-universal```.

    >```setupsolarized ``` must be run at least once in order to create the configuration file. After doing so, the plugin will automatically load your configuration each time a zsh session is started.

- ### Install POWERLEVEL9K and configuration
    - Install fonts

sudo apt-get install powerline fonts-powerline

