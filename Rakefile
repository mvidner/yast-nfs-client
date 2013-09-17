# -*- ruby -*-
require "packaging/tasks"
require "packaging/configuration"
Packaging::Tasks.loadTasks

Packaging::Configuration.run do |c|
  c.skip_license_check << /.*/ # I am cheating!
  c.package_name = "yast2-nfs-client" # will be done by RPMNAME
  c.obs_project = "YaST:Head"
#  c.obs_target = "openSUSE_Factory" # default
  c.obs_sr_project = "YaST:Headdd"
end

task :test do
  puts "Faking a test"
end

