require 'bundler/setup'
require 'opal'

desc 'Build specified dependencies to build dir'
task :dependencies do
	Opal::DependencyBuilder.new(out: 'build').build
end

desc 'Build latest opal-browser-html5-canvas to build dir'
task :build do
	Opal::Builder.new('lib', join: 'build/opal-browser-html5-canvas.js').build
end

task :default => :build
