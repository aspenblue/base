#!/usr/bin/env bash
set -euo pipefail

NEW_CONFIG="/etc/skel/.config"

# set new config
cp -Ra --update=none "$NEW_CONFIG" "$HOME"
    
USER_OWNER=$(stat -c '%U:%G' "$HOME")
chown -R "$USER_OWNER" "$HOME/.config"
