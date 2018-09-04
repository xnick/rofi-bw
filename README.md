# rofi-lpass

Adapted from [rofi-lpass](https://github.com/Mange/rofi-lpass)

Custom script for Rofi that allows you to copy passwords from your Bitwarden vault.

## Features

* List all your entries
* Copy password of an entry
* Copy username / email of an entry
* Copy URL (if entry has an URL)
* Open URL (if entry has an URL)

## Installation

1. Make sure you have [bitwarden-cli](https://github.com/bitwarden/cli/) installed, with `bw` on your `PATH`.
2. Since bw can't copy to clipboard by itself, `xclip` is also needed; should be available in your distro's repo.
3. Symlink the script to somewhere on your `$PATH`: `ln -s $(pwd)/rofi-bw ~/bin/rofi-bw`.
4. Run rofi with this as a custom script: `rofi -modi bw:rofi-bw -show bw`

## License
rofi-lpass: Copyright © 2017 Magnus Bergmark. 

Code released under the MIT license.

