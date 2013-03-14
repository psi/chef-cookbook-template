# encoding: utf-8

require 'bundler'
require 'bundler/setup'
require 'thor/foodcritic'
require 'thor/scmversion'
require 'berkshelf/thor'

class Default < Thor
  desc "release", "Tag a new version and upload to chef-server"
  method_option :type, :default => "patch"
  def release
    invoke "version:bump", [options[:type]]
  end
end
