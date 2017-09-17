require 'html-proofer'

task :test do
  options = { :assume_extension => true }
  HTMLProofer.check_directory("./_site", options).run
end

task :serve do
  sh "bundle exec jekyll serve --watch --config _config.yml,_config_dev.yml"
end

task :build do
  sh "bundle exec jekyll build"
end

task :clean do
  sh "bundle exec jekyll clean"
end
