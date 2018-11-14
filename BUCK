prebuilt_cxx_library(
  name = 'bind',
  header_only = True,
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
  ]),
  deps = [
    'buckaroo.github.buckaroo-pm.boost-config//:config', 
    'buckaroo.github.buckaroo-pm.boost-core//:core', 
    'buckaroo.github.buckaroo-pm.boost-detail//:detail', 
  ], 
  visibility = [
    'PUBLIC',
  ],
)

cxx_binary(
  name = 'bind-as-compose', 
  srcs = [
    'bind_as_compose.cpp', 
  ], 
  deps = [
    ':bind', 
  ], 
)

cxx_binary(
  name = 'bind-visitor', 
  srcs = [
    'bind_visitor.cpp', 
  ], 
  deps = [
    ':bind', 
  ], 
)
