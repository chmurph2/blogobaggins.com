verbose true

desc "Syncs any changes to the actual blog."
task :publish do
  sh("jekyll --pygments --lsi")
  sh("rsync -E --delete --progress -av _site/ blogobaggins.com:blogobaggins.com")
end