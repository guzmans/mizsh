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






🎨 Fonts (Required for Themes)

If you are using a theme like Powerlevel10k or any Oh My Zsh theme that uses special icons,
you need to install a Nerd Font (recommended: MesloLGS Nerd Font - https://github.com/ryanoasis/nerd-fonts).

Download and install the font on your system.

Open your terminal preferences and set the font to the installed Nerd Font.

Without it, you may see broken characters instead of nice icons.

🔌 Plugins

This configuration uses Oh My Zsh, which comes with a plugin system.
If your .zshrc references additional plugins (like zsh-autosuggestions or zsh-syntax-highlighting), install them with:

Mostrar siempre los detalles
# Example: zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions \\\
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

# Example: zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \\\
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting


Then add them to the plugins=(...) section of your ~/.zshrc.

ℹ️ Notes

The chsh command changes your default shell to Zsh.

After running exec zsh, you should see your customized prompt.

If you’re using a non-Debian/Ubuntu distro, install zsh and git with your package manager.

Keep your repo updated with git pull whenever you make changes.
