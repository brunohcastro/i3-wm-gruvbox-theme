Here be almost every file for my personal i3-wm gruvbox theme implementation using the
colors of the great gruvbox color scheme. Good luck!  https://github.com/morhetz/gruvbox



I launch most of my startup programs using .xinitrc except for a script I run
on i3-startup called screens.sh. I run that script whenever i attach/detach
from my external monitor. I also bind it to a hotkey because I have it set to
restart compton and conky, good for debugging/trying out new configs...
Everything else should be plain to see.

I did it in this order:

1. Install Vim gruvbox theme using vim-plug plugin manager.
Enable vim gruvbox theme in vimrc. Source the gruvbox color sh script in
.bashrc or .zshrc since I use URxvt (see my "note-about-terminals"). Lastly, I
installed lightline which will use the vim gruvbox theme also if you have it
enabled in your vimrc. I also have powerline fonts installed along with Hack
and Fantasque Sans Mono.

2. Apply gruvbox 256 color scheme to .Xresources file. Will need to restart X
   server or refresh with Xrdb for this to take immediate effect on new
   terminals.

3. Apply i3 config colors. To all the windows and workspace corner. The two
   sections are at the end of my config file.

4. Apply i3blocks colors. These blocks will not all work the same out of the
   box for everyone. At the least you'll probably need to set your network
   interface for ethernet and wifi will probably be different than mine. (my
   ethernet is 'eno1' and wifi is 'wlp2s0'. Find yours by typing 'ifconfig' or
   'ip link'

5. I am using prezto's zsh config, it's more lightweight than others that are
   out there and by default uses the same colors as gruvbox! Win win.

6. Rofi comes with gruvbox theme included all that is necessary is to turn it
   on.

7. The gtk theme I simply created one to my preferences using oomox. https://github.com/actionless/oomox
I included pictures of my settings and there is also a config file in this
repo. If you make a better one, please share!

Happy grooving.
