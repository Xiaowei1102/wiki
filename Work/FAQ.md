2013/01/06
make menuconfig之后:  
	 缺少这两个文件，touch第二个后，就会全部编译了
        /home/sqm/Documents/flow_md/scripts/config/conf
        /home/sqm/Documents/flow_md/include/config/auto.conf

FPA_RAD_POOL_NUM值，如果不编译radius的话就就少这个宏。
	不管编不编都define一个默认值。

mducmd接口的返回值，在回来之后被设置成了1.

make OpenWRT:
	2013-01-06 18:37:26 (9.64 KB/s) - Read error at byte 14649329/15581509 (Connection timed out). Retrying.
	--2013-01-06 18:37:27--  (try: 2)  http://mirror2.openwrt.org/sources/gdb-6.8.tar.bz2
	Connecting to mirror2.openwrt.org|46.4.11.11|:80... failed: Connection timed out.
	Resolving mirror2.openwrt.org... 46.4.11.11
	Connecting to mirror2.openwrt.org|46.4.11.11|:80... connected.
	HTTP request sent, awaiting response... 206 Partial Content
	Length: 15581509 (15M), 932180 (910K) remaining [application/x-bzip2]
	Saving to: `STDOUT'
	100%[++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++=====>] 15,581,509  8.37K/s   in 1m 44s  
	Could not generate md5sum
	make[3]: *** [/home/sqm/Documents/flow_md/linux/OpenWRT/dl/gdb-6.8.tar.bz2] Error 255
	make[3]: Leaving directory `/home/sqm/Documents/flow_md/linux/OpenWRT/package/gdb'
	make[2]: *** [package/gdb/compile] Error 2
	make[2]: Leaving directory `/home/sqm/Documents/flow_md/linux/OpenWRT'
	make[1]: *** [/home/sqm/Documents/flow_md/linux/OpenWRT/staging_dir/target-mips64-linux/stamp/.package_compile] Error 2
	make[1]: Leaving directory `/home/sqm/Documents/flow_md/linux/OpenWRT'
	make: *** [world] Error 2




2013/01/07
	OCTEON内存对其。
