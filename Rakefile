require 'rake'
require 'rspec/core/rake_task'

task :spec => "spec:all"

namespace :spec do
	RSpec::Core::RakeTask.new(role.to_sym) do |t|
		ENV["ROLE"] = role
		t.pattern = 'spec/#{role}/*_spec.rb'
	end
end

