# ubuntu-gnome-debloated
Debloated Ubuntu ISO image with Vanilla Gnome Desktop made on top of Lubuntu 24.04 LTS ISO

Download from SourceForge: https://sourceforge.net/projects/vanilla-lubuntu-iso/files/

Added Pacstall Support from Rhino Liunx Community: https://pacstall.dev/

	pacstall -S vscode (to search a package)

Changelog:

	Removed all snaps and installed Firefox debian from Mozilla Repository
	
	Removed Ubuntu System reporting tool Apport
	
	Removed Ubuntu Desktop and installed Vanilla Gnome
	
	Removed LXQT Desktop
	
	Installed Gdebi Package Installer
	
	Added Packages- Synaptic,Bleachbit,Gparted,Extension-Manager,VLC,fish
	
	Added Flatpak and Pacstall Suppport
	
Recommended:

	Change default shell to fish after installation by running
	
	chsh
	
	path: /usr/bin/fish
 
 	Install media codecs,fonts (sudo apt install ubuntu-restricted-extras)

	Enable desktop-icons and dock from extension-manager / autologin from settings->users

	Disable snaps install via apt by running
	
	sudo printf "Package: snapd\nPin: release a=*\nPin-Priority: -10" > /etc/apt/preferences.d/nosnap.pref
	
Optional:

	Install ubuntu snap store by running
	
	sudo snap install snap-store
		
	Note: this may install snap dependencies
