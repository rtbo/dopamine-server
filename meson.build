project('dopamine-server', 'd',
    version: '0.1.0-alpha.1',
)

vibed_dep = dependency('vibe-d:http',
    version: '0.9.4',
    method: 'dub',
)

dop_server_src = files([
    'src/dopamine/server/main.d',
])

dop_server_inc = include_directories('src')

dop_server_exe = executable('dop-server', dop_server_src,
    install: true,
    include_directories: dop_server_inc,
    dependencies: vibed_dep,
)
