### drsasimi.github.io Page Repository

#### Prepare Environment

All instructure step is tested on Mac OS X 10.11. other operating system is not tested. :(

1. Install RVM (Ruby Version Manager)

   > curl -sSL https://get.rvm.io | bash -s stable --ruby

2. Check ruby version above 2.1.7

   > $ ruby -version
   >
   > ruby 2.2.1p85 (2015-02-26 revision 49769) [x86_64-darwin14]

   if unmatch ruby version, execute this command

   > $ rvm install 2.2.1
   >
   > $ rvm --default use 2.2.1

3. Install bundles

   > $ gem install bundler

4. Go to directory of `drsasimi.github.io repository` , and create file named `Gemfile` with follow contents.

   ```ruby
   source 'https://rubygems.org'
   gem 'github-pages'
   ```

5. Run follow command on root folder of repository.

   > $ bundle install
   >
   > $ bundle exec jekyll build --safe

6. Create new jekyll site

   > $ jekyll new . --force

7. If you want run server, run this command.

   > $ jekyll serve



