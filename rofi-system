#!/usr/bin/env bash

## rofi-system
## Author: wardxela @ github
## Licence: GPL-3.0

empty_trash() {
  rm -rf ~/.local/share/Trash/*
}

set_volume() {
  wpctl set-volume @DEFAULT_SINK@ "$1"
}

show_options() {
  echo -e "\0prompt\x1fSystem"
  echo -e "Empty Trash\0icon\x1fuser-trash\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
  echo -e "Set Volume to 0%\0icon\x1faudio-volume-muted-symbolic\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
  echo -e "Set Volume to 25%\0icon\x1faudio-volume-low-symbolic\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
  echo -e "Set Volume to 50%\0icon\x1faudio-volume-medium-symbolic\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
  echo -e "Set Volume to 75%\0icon\x1faudio-volume-high-symbolic\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
  echo -e "Set Volume to 100%\0icon\x1faudio-volume-overamplified-symbolic\x1fmeta\x1fSystem\x1fmeta\x1fAudio"
}

case $1 in
  'Empty Trash')
    empty_trash
    exit 0
    ;;
  'Set Volume to 0%')
    set_volume 0
    exit 0
    ;;
  'Set Volume to 25%')
    set_volume 0.25
    exit 0
    ;;
  'Set Volume to 50%')
    set_volume 0.5
    exit 0
    ;;
  'Set Volume to 75%')
    set_volume 0.75
    exit 0
    ;;
  'Set Volume to 100%')
    set_volume 1
    exit 0
    ;;
esac

show_options
exit 0
