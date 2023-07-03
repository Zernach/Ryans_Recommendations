# ryans_recommendations
How I setup my new laptop for programming websites, mobile apps, and data science projects...

## app_dev_checklist
* Install [XCode](https://apps.apple.com/us/app/xcode/id497799835?mt=12), and then open it to accept Terms & Conditions, etc.
* Install [Node Version Manager (NVM)](https://github.com/nvm-sh/nvm)
* Install [Java](https://www.oracle.com/java/technologies/downloads/)
* Install [git](https://git-scm.com/downloads)
* Configure [SSH](http://kbroman.org/github_tutorial/pages/first_time.html)
* Install [VSCode](https://code.visualstudio.com/download) and [Add Code to Path](https://code.visualstudio.com/docs/setup/mac) and install extensions listed at bottom of this ReadMe
* Install [Android Studio](https://developer.android.com/studio)
* Install [Node.js](https://coolestguidesontheplanet.com/installing-node-js-on-macos/) & brew install npm & [grant npm permission](https://stackoverflow.com/questions/51967335/npm-install-permission-denied-macos/57777299#57777299)
* Install [Watchman](https://facebook.github.io/watchman/docs/install#buildinstall)
* Install [Expo](https://docs.expo.io/get-started/installation/), register, and login

## ryans_software_selections
* Chrome
* Zoom
* Visual Studio Code
* Android Studio
* MacBook App Store:
    * Slack 
    * XCode
    * Transporter
    * The Unarchiver
    * iMovie
    * Paint S
    * WhatsApp
    * Capto: Screen Capture & Recording 

## Other random tips
* VSCode Extensions
   * Bracket Pair Colorizer
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

## Scripts
```
# install homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# install oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# install asdf
brew install asdf
echo -e "\n. \"$(brew --prefix asdf)/libexec/asdf.sh\"" >> ~/.bash_profile
echo -e "\n. \"$(brew --prefix asdf)/etc/bash_completion.d/asdf.bash\"" >> ~/.bash_profile

brew install git
brew install yarn
brew install --cask visual-studio-code
brew install --cask android-studio
brew install --cask react-native-debugger

```
