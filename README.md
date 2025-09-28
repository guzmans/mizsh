# My Zsh Configuration

This repository contains my **Zsh** setup along with **Oh My Zsh**.

## 🚀 Installation

On a new machine, run the following steps:

```bash
# Install Zsh and Git
sudo apt update && sudo apt install -y zsh git

# Clone this repository
git clone https://github.com/guzmans/zsh-config.git ~/mizsh

# Copy configuration to your home directory
cp ~/mizsh/.zshrc ~/
cp -r ~/mizsh/.oh-my-zsh ~/

# Change the default shell to Zsh
chsh -s $(which zsh)

# Start Zsh
exec zsh
