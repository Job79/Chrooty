# Chrooty
Minimal chroot manager

# Features
- Download and manage chroot images
- Create and manage chroots
- Run commands inside a chroot
- Export chroots as an image
- Create chroots with build scripts

# Usage 
	chrooty v2.0; chroot manager

	USAGE
		chrooty command [args...]

	COMMANDS
		pull [url<:name>]			download image from repository
		images					list local images
		rmimage [images...]			remove local image

		create [chroot] [image]			create new chroot fom image
		run [chroot] [command] [<args>...]	run command in a chroot
		chroots					list local chroots
		rmchroot [chroots...]			remove local chroot
		export [chroot] [<image>]		export chroot to image



	chrooty builder v2.0; build chroot images 

	USAGE
		builder command [args...]

	COMMANDS
		build [image] 				build chroot image
		import [image<:name>]			move image to local image dir
		images					list all available images
		clean					remove all build images

	BUILD SCRIPT FUNCTIONS
		FROM					use another image as base image
		EXEC					chroot and execute command inside rootfs

	IMAGE FORMAT
	├──rootfs 					chroot filesystem
	├──<before-chroot>				executed on host before chroot
	├──<chroot>					executed inside chroot
	└──<after-chroot>				executed on host after chroot
