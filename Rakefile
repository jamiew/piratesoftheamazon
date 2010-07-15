task :default => :build
 
desc 'Build site'
task :build do
  sh 'rm -f googlealarm.xpi'
  sh "zip pirates-of-the-amazon.xpi -r chrome.manifest content install.rdf" # works on linux + mac
end

task :install => :build do
  sh 'open -a Firefox pirates-of-the-amazon.xpi' # mac-oriented
end
 
