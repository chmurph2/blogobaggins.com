verbose true
task :publish do
  sh("rsync -E --delete --progress -av "_site/" blogobaggins.com:blogobaggins.com")
end