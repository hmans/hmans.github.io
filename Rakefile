task default: [:build]

desc "Build the website"
task :build do
  system "rm -rf _build/* && bin/flutterby build"
end

desc "Deploy the website"
task deploy: [:build] do
  system "scp -r _build/* hmans@sunder:/var/www/hmans.io/"
end