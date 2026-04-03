Rio Harapan Personal blog.

This weblog theme is inspired by [Kiko](http://github.com/gfjaru/Kiko) theme with some modification.

$ brew install rbenv
$ rbenv install 3.2.6
$ rbenv local 3.2.6

Then add this to ~/.zshrc:

$ echo 'eval "$(rbenv init - zsh)"' >> ~/.zshrc
$ source ~/.zshrc

Verify:

$ ruby --version
$ bundle install
$ bundle exec jekyll serve