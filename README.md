# Chrooty
Minimal chroot manager

# Features
- Download and manage chroot images (chroot as .tar.gz)
- Create and manage chroots
- Run commands inside a chroot
- Export chroots as an image

# Usage 
	chrooty v1.0; chroot manager

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
