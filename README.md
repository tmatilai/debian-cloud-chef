# Chef installer plugin for build-debian-cloud

This [build-debian-cloud](https://github.com/andsens/build-debian-cloud)
plugin installs Opscode Chef client using the [Omnibus installer]
(http://www.opscode.com/chef/install/). It also installs rsync to support e.g.
[Vagrant AWS Provider](https://github.com/mitchellh/vagrant-aws) and
[knife-solo](http://matschaffer.github.io/knife-solo/).

*Until the Omnibus Chef installer supports Debian 7.0 Wheezy, this plugin only
works on Debian 6.0 Squeeze. Check out the [wheezy branch]
(https://github.com/tmatilai/debian-cloud-chef/tree/wheezy) if you want to use
the Squeeze package for Wheezy.*


## Usage

To install the plugin, download and extract the [tarball]
 (https://github.com/tmatilai/debian-cloud-chef/archive/master.tar.gz)
or clone the [git repository](https://github.com/tmatilai/debian-cloud-chef).
Then pass the plugin to build-debian-cloud:

    ./build-debian-cloud (ec2 | gce) --plugin <path_to>/debian-cloud-chef/install-chef

By default the latest stable release of Chef client is installed.
`$CHEF_VERSION` environment variable can be used to specify another version.
