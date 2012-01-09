require 'bundler/setup'
require 'opal'

desc 'Build specified dependencies into .'
task :dependencies do
	Opal::DependencyBuilder.new(dependencies: %w[opal-browser opal-spec], out: 'build').build
end

desc 'Build latest opal-browser-html5-canvas to current dir'
task :browser do
	Opal::Builder.new('lib', join: 'build/opal-browser-html5-canvas.js').build
end

task :default => :browser
