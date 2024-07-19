transcoder_sources = [
  'main.vala',
  'application.vala',
  'window.vala',
]

transcoder_deps = [
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

transcoder_sources += gnome.compile_resources('transcoder-resources',
  'transcoder.gresource.xml',
  c_name: 'transcoder'
)

executable('transcoder', transcoder_sources,
  dependencies: transcoder_deps,
       install: true,
)
