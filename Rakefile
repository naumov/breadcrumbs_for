require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "breadcrumbs_for"
    gem.summary = %Q{Breadcrumbs Rails helper.}
    gem.description = %Q{Breadcrumbs helper for Rails done in a rails way. Built on url_for, your routes, model names and i18n.}
    gem.email = "naumovmail@gmail.com"
    gem.homepage = "http://github.com/naumov/breadcrumbs_for"
    gem.authors = ["Dmitry Naumov"]
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

task :test => :check_dependencies

task :default => :test

require 'rake/rdoctask'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "breadcrumbs_for #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end