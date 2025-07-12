<h3>Install some packages</h3>
```yay -S wl-clipboard cliphist light grim slurp rofi waybar pavucontrol arc-gtk-theme network-manager-applet nm-connection-editor```

<h3>Network</h3>
turn on network manager and add user to the group
```sudo systemctl enable --now NetworkManager```
```sudo usermod -aG network $USER```

<h3>Set dark theme</h3>
```gsettings set org.gnome.desktop.interface gtk-theme 'Arc-Dark'```

<h3>Rofi</h3>
you need to move rofi folder into ~/.config
```cp -r ./rofi ~/.config/```

<h3>Chinese characters</h3>
```sh
yay -S noto-fonts-cjk adobe-source-han-sans-cn-fonts adobe-source-han-serif-cn-fonts wqy-microhei
```
```sudo vim /etc/locale.gen```

uncomment:
zh_CN.UTF-8 UTF-8
zh_TW.UTF-8 UTF-8
en_US.UTF-8 UTF-8

```sh
sudo locale-gen

