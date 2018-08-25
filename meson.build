project('enkiTS', 'cpp')
cpp_sources = [
    'src/Atomics.h',
    'src/LockLessMultiReadPipe.h',
    'src/TaskScheduler.cpp',
    'src/TaskScheduler.h',
    'src/Threads.h'
]
thread_dep = dependency('threads')
l = static_library('enkiTS', cpp_sources,
    dependencies: thread_dep)
i = include_directories('src')
enkiTS_dep = declare_dependency(include_directories: i,
    link_with: l)
