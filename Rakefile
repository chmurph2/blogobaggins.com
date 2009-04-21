verbose true

task :default => :server

desc "Launches the jekyll server."
task :server do
  sh("jekyll --server")
end

desc "Syncs any changes to the actual blog."
task :publish do
  sh("jekyll --no-auto")
  sh("rsync -E --delete --progress -av _site/ blogobaggins.com:blogobaggins.com")
end