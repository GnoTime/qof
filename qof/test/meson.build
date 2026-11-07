test_deps = [
  glib_dep,
]

# test-book-merge

test_book_merge_srcs = files(
  'test-book-merge.c',
  'test-stuff.c',
)

qof_test_book_merge = executable('qof-test-book-merge',
  test_book_merge_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-book-merge',
  qof_test_book_merge,
)

# test-date

test_date_srcs = files(
  'test-date.c',
  'test-stuff.c',
)

qof_test_date = executable('qof-test-date',
  test_date_srcs,
  c_args: ['-D_DEFAULT_SOURCE', '-D_XOPEN_SOURCE'],
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-date',
  qof_test_date,
)

# test-event

test_event_srcs = files(
  'test-event.c',
  'test-engine-stuff.c',
  'test-stuff.c',
)

qof_test_event = executable('qof-test-event',
  test_event_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-event',
  qof_test_event,
)

# test-guid

test_guid_srcs = files(
  'test-guid.c',
  'test-stuff.c',
)

qof_test_guid = executable('qof-test-guid',
  test_guid_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-guid',
  qof_test_guid,
)

# test-numeric

test_numeric_srcs = files(
  'test-numeric.c',
  'test-stuff.c',
)

qof_test_numeric = executable('qof-test-numeric',
  test_numeric_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-numeric',
  qof_test_numeric,
)

# test-object

test_object_srcs = files(
  'test-object.c',
  'test-stuff.c',
)

qof_test_object = executable('qof-test-object',
  test_object_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-object',
  qof_test_object,
)

# test-querynew

test_querynew_srcs = files(
  'test-querynew.c',
  'test-stuff.c',
)

qof_test_querynew = executable('qof-test-querynew',
  test_querynew_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-querynew',
  qof_test_querynew,
)

# test-recursive

test_recursive_srcs = files(
  'test-engine-stuff.c',
  'test-recursive.c',
  'test-stuff.c',
)

qof_test_recursive = executable('qof-test-recursive',
  test_recursive_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-recursive',
  qof_test_recursive,
)

# test-sql

test_sql_srcs = files(
  'test-sql.c',
  'test-stuff.c',
)

qof_test_sql = executable('qof-test-sql',
  test_sql_srcs,
  dependencies: test_deps,
  include_directories: [config_inc, libqof_inc],
  link_with: libqof,
)

test('qof-test-sql',
  qof_test_sql,
)
