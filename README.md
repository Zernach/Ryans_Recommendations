# ryans_recommendations
How I setup my machines for mobile app development and web development.

## ⚙️ <u>Scripts</u>
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
brew install nvm
brew install yarn
brew install watchman
brew install openjdk
brew install --cask google-chrome
brew install --cask visual-studio-code
brew install --cask android-studio
brew install --cask react-native-debugger
brew install --cask capto
brew install --cask whatsapp
brew install --cask slack
brew install --cask rectangle

```

## ⚙️ <u>Additional Steps</u>
* Configure [SSH](http://kbroman.org/github_tutorial/pages/first_time.html)
* After installing VSCode, [add Code to Path](https://code.visualstudio.com/docs/setup/mac) and install extensions listed at bottom of this ReadMe
* Install [Expo](https://docs.expo.io/get-started/installation/), register, and login

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
