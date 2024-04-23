# 📱 Mobile App Development Installation Guide
💻 Everything Needed for React Native Mobile App Development on a New Laptop

<br/>
<br/>

## ⚙️ <u>Scripts</u>

1. Install HomeBrew (when finished installing, copy the two lines of code in your terminal and run them to add HomeBrew initialization scripts to your shell)
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Use HomeBrew to Install Stuff
```sh
brew tap wix/brew; 
brew install git nvm yarn watchman openjdk applesimutils cocoapods ios-deploy asdf expo-orbit pyenv hasura-cli; 
brew install --cask reactotron google-chrome visual-studio-code android-studio react-native-debugger vpn-by-google-one surfshark kap whatsapp slack zoom rectangle steam; 
```

3. Install oh-my-zsh
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

4. Add Lines to Your ./.zshrc File
```sh
echo -e "\n\n\"$(brew --prefix asdf)/libexec/asdf.sh\"\n\n\"$(brew --prefix asdf)/etc/bash_completion.d/asdf.bash\" \n\neval "$(/opt/homebrew/bin/brew shellenv)" \n\nsource ~/.nvm/nvm.sh" >> ~/.zshrc;
echo 'export PATH="/opt/homebrew/opt/openjdk/bin:$PATH"' >> ~/.zshrc
```

5. Use npm to Globally Install Some SDK's
```sh
npm install -g react-native-cli @react-native-community/cli expo-cli lint-staged create-expo-app ignite-cli@lates
```

6. Login to Expo
```sh
expo login
```

<br/>
<br/>

## ⚙️ <u>Manual Steps</u>
1. Create your SSH key by individually running the following commands and your replacing your first/last name and email address for use with Github/GitLab/Bitbucket:

<br/>

`git config --global user.name "FirstName LastName"`

<br/>

`git config --global user.email "your_email@example.com"`

<br/>

`ssh-keygen -t rsa -C "your_email@example.com"`

<br/>

2. Add your newly-created SSH key to GitHub/GitLab/BitBucket by copying the new key to your clipboard with `pbcopy < ~/.ssh/id_rsa.pub`, and then paste the key's value into GitHub/GitLab/BitBucket SSH key settings.
3. Open VSCode and add code to path by pressing command-shift-p, searching for "install code", and select the `Shell Command: Install 'code' command in PATH` option
4. Uninstall VSCode Extensions so you can install the newest versions in the next step.
```sh
code --uninstall-extension CoenraadS.bracket-pair-colorizer-2;
code --uninstall-extension Orta.vscode-jest;
code --uninstall-extension naumovs.color-highlight;
code --uninstall-extension vangware.dark-plus-material;
code --uninstall-extension rodrigovallades.es7-react-js-snippets;
code --uninstall-extension GitHub.copilot GraphQL.vscode-graphql;
code --uninstall-extension orsenkucher.vscode-graphql;
code --uninstall-extension ms-toolsai.jupyter-keymap;
code --uninstall-extension ms-toolsai.jupyter-renderers;
code --uninstall-extension ms-toolsai.jupyter;
code --uninstall-extension ritwickdey.LiveServer;
code --uninstall-extension PKief.material-icon-theme;
code --uninstall-extension rvest.vs-code-prettier-eslint;
code --uninstall-extension ms-python.vscode-pylance ms-python.python;
code --uninstall-extension msjsdiag.vscode-react-native;
code --uninstall-extension alexcvzz.vscode-sqlite tomoki1207.pdf;
code --uninstall-extension eamodio.gitlens;
code --uninstall-extension ms-azuretools.vscode-docker;
```
5. Install VSCode Extensions
```sh
code --install-extension CoenraadS.bracket-pair-colorizer-2;
code --install-extension Orta.vscode-jest naumovs.color-highlight;
code --install-extension vangware.dark-plus-material;
code --install-extension rodrigovallades.es7-react-js-snippets;
code --install-extension GitHub.copilot GraphQL.vscode-graphql;
code --install-extension orsenkucher.vscode-graphql ms-toolsai.jupyter-keymap;
code --install-extension ms-toolsai.jupyter-renderers;
code --install-extension ms-toolsai.jupyter ritwickdey.LiveServer;
code --install-extension PKief.material-icon-theme;
code --install-extension rvest.vs-code-prettier-eslint;
code --install-extension ms-python.vscode-pylance;
code --install-extension ms-python.python;
code --install-extension msjsdiag.vscode-react-native alexcvzz.vscode-sqlite;
code --install-extension tomoki1207.pdf;
code --install-extension eamodio.gitlens;
code --install-extension ms-azuretools.vscode-docker;
```
6. Downloads from MacBook App Store:
    * XCode
    * Transporter
    * The Unarchiver
    * iMovie
    * Paint S

<br/>
<br/>

## ⚙️ <u>XCode Setup</u>
Next make sure [XCode from the MacBook App Store](https://apps.apple.com/us/app/xcode/id497799835?mt=12) is installed and up to date. You may also want to ensure that your MacBook's operating system is up-to-date before installing/updating XCode. Upon installing XCode, there some additional setup required so that React Native can interact with the XCode command line interface toolkit:
1. Launch XCode
2. Go to `Xcode` | `Settings` in the menu bar
3. Go to `Locations` in the preferences window
4. Click the drop down next to `Command Line Tools` and select the version of Xcode you are currently using. There is most likely a set of `Command Line Tools` already selected, but you should re-select the same selection to ensure that it properly engages.

<br/>
<br/>

## ⚙️ <u>Android Studio Setup</u>
* After installing Android Studio using HomeBrew above, there's some additional setup required:
1. Open Android Studio, and on the main home screen, click `More Actions` dropdown and select `SDK Manager`
2. Check the box next to `Android SDK Command-line Tools (latest)`
3. Finally, click Apply and then Ok, accept license agreements as needed
After installing everything in the above steps, then make sure the following environment variables are in your `~/.zshrc` file (or `~/.bashrc` file if you use `bash`) — **but it's important that you replace "yourUsername" below with your actual laptop's username:**

```
export ANDROID_SDK=/Users/yourUsername/Library/Android/sdk
export ANDROID_SDK_ROOT=/Users/yourUsername/Library/Android/sdk
export ANDROID_HOME=/Users/yourUsername/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```
