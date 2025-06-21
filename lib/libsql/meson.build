lex = find_program('lex', 'flex')
yacc = find_program('yacc', 'bison')

parser_c = custom_target('parser_c',
  command: [yacc, '-v', '-d', '-o', '@OUTPUT@', '-p', 'sql', '@INPUT@'],
  input: 'parser.y',
  output: 'parser.c',
)

lexer_c = custom_target('lexer_c',
  command: [lex, '-o@OUTPUT@', '-Psql', '@INPUT@'],
  depends: parser_c,
  input: 'lexer.l',
  output: 'lexer.c',
)

libqofsql_deps = [
  glib_dep,
]

libqofsql_srcs = files(
  'mem.c',
  'sql_display.c',
  'sql_parser.c',
  'sql_tree.c',
)
libqofsql_srcs += [
  lexer_c,
  parser_c,
]

libqofsql = library('libqofsql',
  dependencies: libqofsql_deps,
  sources: libqofsql_srcs,
)

libqofsql_inc = include_directories('.')
