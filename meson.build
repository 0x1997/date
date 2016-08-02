project('date', 'cpp')

inc = include_directories('.', is_system: true)

install_headers(
    'chrono_io.h',
    'date.h',
    'islamic.h',
    'iso_week.h',
    'julian.h',
    'tz.h',
    'tz_private.h',
    subdir: 'date'
)

lib = static_library('date',
    'tz.cpp',
    cpp_args: [
        '-DHAS_REMOTE_API=0',
        '-Wno-unused-function',
    ],
    pic: true,
)
