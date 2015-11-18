# beegfs-kmod.el6
Building the beegfs-client kernel module for RHEL6/clones

Initial version built for CentOS-6.7 2.6.32-573.el6

Work based on the elrepo/templates/el6 at https://github.com/elrepo/templates.git

Disable the autobuild feature:
# sed -i -e 's/^buildEnabled=true/buildEnabled=false/g' /etc/beegfs/beegfs-client-autobuild.conf

The sources have been pulled by doing:

# rpm2cpio beegfs-client-2015.03.r7-el6.noarch.rpm | cpio -iudv
# cd opt/beegfs/src/client && tar cjvf beegfs-2015.03.r7.tar.bz2 beegfs_client_module_2015.03

YMMV, use at your own risks.

Tru
