imageorgmp_sources = [
  'main.c',
  'imageorgmp-window.c',
]

imageorgmp_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk+-3.0', version: '>= 3.22'),
]

gnome = import('gnome')

imageorgmp_sources += gnome.compile_resources('imageorgmp-resources',
  'imageorgmp.gresource.xml',
  c_name: 'imageorgmp'
)

executable('imageorgmp', imageorgmp_sources,
  dependencies: imageorgmp_deps,
  install: true,
)
