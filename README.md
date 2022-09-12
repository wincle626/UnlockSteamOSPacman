# This is a simple way to unlock the pacman on SteamOS

This applies to Desktop Mode.

    If you have not already, use passwd to create a password for the deck user.

    Disable read-only mode: sudo btrfs property set -ts / ro false

    Initialize the pacman keyring: sudo pacman-key --init

    Populate the pacman keyring with the default Arch Linux keys: sudo pacman-key --populate archlinux

    Try installing a package: sudo pacman -S vi

Note that any packages you install will likely be overwritten by the next Steam Deck update.
