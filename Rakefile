task :doc do
  sh %{rdoc --all --one-file}
end

namespace :run do
  task :spec do
    sh %{rspec visitor_spec.rb}
  end
end

namespace :clean do
  task :all => [:doc]
  task :doc do
    sh %{rm -rf doc/}
  end
end