# redot-flatpak
My attempt at a Redot Flatpak. This is my first Flatpak, I'm unsure how well it is made or if it works well. Credit to Godot's Flatpak for some code.\
Currently having big filesystems issues with importing, and when opening a project, small error screen.

build w:
flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir org.redotengine.Redot.yml

run w: (change sockets to what you use, such as wayland)
flatpak run --socket=x11 --socket=pulseaudio --filesystem=host --share=network --device=all --talk-name=org.freedesktop.Flatpak org.redotengine.Redot
