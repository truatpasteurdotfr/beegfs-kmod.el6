# beegfs-kmod.el6
Building the beegfs-client kernel module for RHEL6/clones

Initial version built for CentOS-6.7 2.6.32-573.el6

sed -i -e 's/^buildEnabled=true/buildEnabled=false/g' /etc/beegfs/beegfs-client-autobuild.conf
