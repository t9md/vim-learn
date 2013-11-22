OUTPUT="README.html"
desc "default"
task :default do
  sh "pandoc README.md -s -o #{OUTPUT} -c github.css"
  sh "open #{OUTPUT}"
end

desc "clean"
task :clean do
  sh "rm -f #{OUTPUT}"
end
