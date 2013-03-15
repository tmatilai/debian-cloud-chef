# Chef installer plugin for ec2debian-build-ami

This [ec2debian-build-ami](https://github.com/andsens/ec2debian-build-ami)
plugin installs Opscode Chef client using the [Omnibus installer]
(http://www.opscode.com/chef/install/).

*Until the Omnibus Chef installer supports wheezy, this plugin only works on
Debian squeeze.*

## Usage

To install the plugin, download and extract the [tarball]
 (https://github.com/tmatilai/ec2debian-chef/archive/master.tar.gz)
or clone the [git repository](https://github.com/tmatilai/ec2debian-chef).
Then pass the plugin to ec2debian-build-ami:

    ./ec2debian-build-ami --plugin <path_to>/ec2debian-chef/install-chef
