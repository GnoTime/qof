cc = meson.get_compiler('c')
m_dep = cc.find_library('m')

libqof_deps = [
  glib_dep,
  gmodule_dep,
  gobject_dep,
  m_dep,
]

libqof_srcs = files(
   'guid.c',
   'kvpframe.c',
   'kvputil.c',
   'md5.c',
   'qofbackend.c',
   'qofbook.c',
   'qofbookmerge.c',
   'qofchoice.c',
   'qofclass.c',
   'qofdate.c',
   'qoferror.c',
   'qofevent.c',
   'qofgobj.c',
   'qofid.c',
   'qofinstance.c',
   'qoflog.c',
   'qofnumeric.c',
   'qofobject.c',
   'qofquery.c',
   'qofquerycore.c',
   'qofreference.c',
   'qofsession.c',
   'qofsql.c',
   'qofstrftime.c',
   'qofstrptime.c',
   'qoftime.c',
   'qofundo.c',
   'qofutil.c',
)

libqof = library('libqof',
  c_args: '-DQOF_LIB_DIR="' + join_paths(get_option('prefix'), get_option('libdir'), package + soname) + '"',
  dependencies: libqof_deps,
  include_directories: [config_inc, libqofsql_inc],
  link_with: libqofsql,
  sources: libqof_srcs,
)

libqof_inc = include_directories('.')
