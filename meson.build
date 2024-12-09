project('mamolinux-keyring',
  version: run_command('head', '-1', 'debian/changelog', check: true).stdout().split(' ')[1].strip('(').strip(')'),
  license: ['GPL3'],
  default_options : ['warning_level=3',
    'prefix=/usr',
  ]
)

prefix = get_option('prefix')
datadir = get_option('datadir')

subdir('data')
