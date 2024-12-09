keyring_dir = join_paths(datadir, 'keyrings')

gpgkeys = []
gpgkeys += files(
	run_command(
		'find',
		meson.current_source_dir(),
		'-name', '*.gpg',
		check: true
	).stdout().strip().split('\n')
)

foreach key: gpgkeys
	install_data(key,
		install_dir: keyring_dir,
	)
endforeach
