# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)
require 'rake'
require 'resque/tasks'
require 'resque_scheduler/tasks'
task "resque:scheduler_setup" => :environment # load the env so we know about the job classes
include Rake::DSL
Openkeywords::Application.load_tasks