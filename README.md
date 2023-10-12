# ryans_recommendations
How I setup my machines for mobile app development and web development.

## ⚙️ <u>Scripts</u>
```sh
# install homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# install oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

brew tap wix/brew
brew install git nvm yarn watchman openjdk applesimutils cocoapods
brew install --cask asdf google-chrome visual-studio-code android-studio react-native-debugger vpn-by-google-one kap whatsapp slack zoom rectangle steam

npm install -g react-native-cli @react-native-community/cli expo-cli

expo login

```

## ⚙️ <u>.zshrc</u>
```sh
echo -e "\n. \"$(brew --prefix asdf)/libexec/asdf.sh\"" >> ~/.bash_profile
echo -e "\n. \"$(brew --prefix asdf)/etc/bash_completion.d/asdf.bash\"" >> ~/.bash_profile
source ~/.nvm/nvm.sh
```

## ⚙️ <u>Additional Steps</u>
* Configure [SSH](http://kbroman.org/github_tutorial/pages/first_time.html)
* After installing VSCode, [add Code to Path](https://code.visualstudio.com/docs/setup/mac) and install extensions listed at bottom of this ReadMe
* After installing Android Studio, there's some additional setup required:
1. Open Android Studio
2. On the main home screen, click `More Actions` dropdown and select `SDK Manager`
3. Check the box next to `Android SDK Command-line Tools (latest)`
4. Switch to the `SDK Platforms` tab
5. Check the box next to `Android 12L (Sv2)`
6. Check the `Show Package Details` box at the bottom of the screen
7. Under the Android 12L (Sv2) section check the box `Google APIs Intel x86 Atom_64 System Image`
8. Finally, click Apply and then Ok, accept license agreements as needed
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

Next make sure [XCode from the MacBook App Store](https://apps.apple.com/us/app/xcode/id497799835?mt=12) is installed and up to date. Upon installing, XCode also requires some additional setup so that React Native can interact with the XCode command line interface toolkit:
1. Launch XCode
2. Go to `Xcode` | `Settings` in the menu bar
3. Go to `Locations` in the preferences window
4. Click the drop down next to `Command Line Tools` and select the version of Xcode you are currently using.

## ⚙️ <u>MacBook App Store</u>
* XCode and then open it to accept Terms & Conditions, and select XCode Command Line Tools version
* Transporter
* The Unarchiver
* iMovie
* Paint S

## ⚙️ <u>VSCode Extensions</u>
* Bracket Pair Colorizer
* Jest
* Color Highlight
* Dark+ Material
* ES7 React/Redux/GraphQL
* Github Copilot
* GraphQL: Language Feature Support
* GraphQL: Syntax Highlighting
* Jupyter
* Jupyter Keymap
* Jupyter Notebook Renderers
* Live Server
* Material Icon Theme
* Prettier ESLint
* Pylance
* Python
* React Native Tools
* SQLite
* vscode-pdf
