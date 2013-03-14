# encoding: utf-8

require 'bundler'
require 'bundler/setup'
require 'thor/foodcritic'
require 'thor/scmversion'
require 'berkshelf/thor'

class Default < Thor
  desc "release", "Tag a new version and upload to chef-server"
  def release
    invoke "version:bump", ["patch"]
  end
end
