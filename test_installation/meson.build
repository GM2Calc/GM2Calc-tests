project('example', ['c','cpp'], default_options: ['cpp_std=c++11'])

add_project_link_arguments(['-lstdc++','-lm'], language : 'c')

deps = [dependency('gm2calc')]

executable('example', 'example.cpp', dependencies: deps)
executable('example-c', 'example.c', dependencies: deps)
