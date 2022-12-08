project(
    'vtparse',
)

ruby = find_program('ruby', required: true)

run_command('make', 'lib', check: true, env: ['RUBYLIB=.'])


cc = meson.get_compiler('c')
vtparse_dep = declare_dependency(
    dependencies: cc.find_library('vtparse', dirs: meson.current_source_dir()),
    include_directories: '.',
)
