project('ssifbridge', 'c',
    default_options: [
        'buildtype=debugoptimized',
        'warning_level=3',
        'werror=true',
    ],
    version: '1.0',
)

add_project_arguments('-Wno-psabi', language: 'c')

deps = [dependency('libsystemd', version : '>=221'),
        dependency('systemd'),
]

executable('ssifbridged','ssifbridged.c',
           dependencies: deps,
           install: true)
