# redot-flatpak
My attempt at a Redot Flatpak. This is my first Flatpak, I'm unsure how well it is made or if it works well

build w:
flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir org.redotengine.Redot.yml

run w:
flatpak run --socket=x11 --socket=pulseaudio org.redotengine.Redot
