Package build:

perl otrs.PackageManager.pl -a build -p %GitHome%\cbs_Menu_items_OTRS\cbs_menu_items.sopm -d %GitHome%\cbs_Menu_items_OTRS\

perl otrs.PackageManager.pl -a build -p /home/github/cbs_Menu_items_OTRS/cbs_menu_items.sopm -d /home/github/cbs_Menu_items_OTRS/

Install:

su -s /bin/bash -c "/opt/otrs/bin/otrs.PackageManager.pl -a install -p /tmp/cbs_menu_items-0.1.5.opm" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.RebuildConfig.pl" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.DeleteCache.pl" otrs


Uninstall:

su -s /bin/bash -c "/opt/otrs/bin/otrs.PackageManager.pl -a uninstall -p cbs_menu_items" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.RebuildConfig.pl" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.DeleteCache.pl" otrs

Update:

su -s /bin/bash -c "/opt/otrs/bin/otrs.PackageManager.pl -a upgrade -p /tmp/cbs_menu_items-0.1.5.opm" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.RebuildConfig.pl" otrs
su -s /bin/bash -c "/opt/otrs/bin/otrs.DeleteCache.pl" otrs
