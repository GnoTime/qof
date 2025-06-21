sqlite_req = '>= 2.8.0'

sqlite_dep = dependency('sqlite', version: sqlite_req)

libqof_backend_sqlite_deps = [
  glib_dep,
  sqlite_dep,
]

libqof_backend_sqlite_srcs = files(
  'qof-sqlite.c',
)

library('libqof_backend_sqlite',
  c_args: '-DLOCALE_DIR="' + join_paths(get_option('prefix'), get_option('localedir')) + '"',
  dependencies: libqof_backend_sqlite_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
  sources: libqof_backend_sqlite_srcs,
)
