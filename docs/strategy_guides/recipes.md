# Recipes

!> :construction: This page is **under construction**, expect frequent major
updates and corrections until this banner is removed. :construction:

> Recipes are a lesser-known term given to short specific series of actions that
> give an specific outcome with a narrowly defined scope. An example of
> something that _is_ a recipe would be "Factory resetting the Steam Deck". An
> example of something that _is not_ a recipe would be "When to reset your Steam
> Deck"

- [Recipes](#recipes)
  - [Activate Root Access](#activate-root-access)
  - [Enable SSH](#enable-ssh)

## Activate Root Access

1. Open a terminal window (Konsole) and begin the process of setting a password
   by issuing the command `passwd`

   ```bash
   $ passwd
   New password:
   Re-enter new password:

   ```

2. Enter your desired terminal password twice to confirm
   > Note that it will not show any characters as you type
3. The default OS username of the Steam Deck is currently `deck`, irrespective
   of which Steam user is logged in

## Enable SSH

1. If you haven't already, [Activate Root Access](#activate-root-access)
2. Enable the ssh system service `sudo systemctl enable sshd --now`
3. Find IP address `ip addr |grep dynamic`
   > Example:
   > ` inet 192.168.1.194/24 brd 192.168.1.255 scope global dynamic noprefixroute wlan0`
4. Connect from your client `ssh deck@192.168.1.194`
