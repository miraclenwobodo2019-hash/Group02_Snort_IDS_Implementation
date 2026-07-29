┌──(kali㉿kali)-[~]
└─$ ~/snort_src/snort3/build
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ make -j$(nproc)
[  0%] Built target unixdomain_connector
[  2%] Built target framework
[  2%] Built target mp_unix_transport
[  3%] Built target ips_actions
[  3%] Built target codecs
[  3%] Built target root_codecs
[  4%] Built target link_codecs
[  6%] Built target ip_codecs
[  7%] Built target misc_codecs
[  7%] Built target control
[ 10%] Built target detection
[ 10%] Built target dump_config
[ 11%] Built target events
[ 13%] Built target file_api
[ 13%] Built target filter
[ 14%] Built target flow
[ 15%] Built target hash
[ 16%] Built target js_norm
[ 16%] Built target latency
[ 17%] Built target log
[ 19%] Built target main
[ 20%] Built target managers
[ 21%] Built target memory
[ 22%] Built target mime
[ 23%] Built target packet_io
[ 24%] Built target parser
[ 25%] Built target payload_injector
[ 26%] Built target ports
[ 27%] Built target protocols
[ 27%] Built target sfip
[ 27%] Built target sfrt
[ 27%] Built target service_inspectors
[ 27%] Built target back_orifice
[ 29%] Built target cip
[ 32%] Built target dce_rpc
[ 32%] Built target dnp3
[ 34%] Built target dns
[ 35%] Built target ftp_telnet
[ 36%] Built target gtp_inspect
[ 40%] Built target http_inspect
[ 42%] Built target http2_inspect
[ 43%] Built target iec104
[ 43%] Built target imap
[ 44%] Built target mms
[ 44%] Built target modbus
[ 44%] Built target netflow
[ 45%] Built target opcua
[ 45%] Built target pop
[ 45%] Built target rpc_decode
[ 46%] Built target s7commplus
[ 47%] Built target sip
[ 47%] Built target smtp
[ 47%] Built target ssh
[ 48%] Built target ssl
[ 48%] Built target tlv_pdu
[ 50%] Built target wizard
[ 51%] Built target socks
[ 51%] Built target stream
[ 52%] Built target stream_paf
[ 52%] Built target stream_base
[ 52%] Built target stream_ip
[ 52%] Built target stream_icmp
[ 55%] Built target stream_tcp
[ 56%] Built target stream_udp
[ 56%] Built target stream_user
[ 57%] Built target stream_file
[ 57%] Built target target_based
[ 58%] Built target host_tracker
[ 59%] Built target pub_sub
[ 60%] Built target time
[ 61%] Built target profiler
[ 61%] Built target trace
[ 62%] Built target tracer
[ 62%] Built target utils
[ 63%] Built target helpers
[ 63%] Built target lua
[ 63%] Built target decompress
[ 69%] Built target ips_options
[ 70%] Built target loggers
[ 70%] Built target network_inspectors
[ 78%] Built target appid
[ 78%] Built target arp_spoof
[ 78%] Built target binder
[ 79%] Built target extractor
[ 79%] Built target normalize
[ 79%] Built target packet_capture
[ 80%] Built target perf_monitor
[ 80%] Built target port_scan
[ 80%] Built target reputation
[ 82%] Built target rna
[ 82%] Built target policy_selectors
[ 82%] Built target address_space_selector
[ 82%] Built target tenant_selector
[ 83%] Built target search_engines
[ 84%] Built target side_channel
[ 84%] Built target connectors
[ 84%] Built target file_connector
[ 84%] Built target tcp_connector
[ 84%] Built target std_connector
[ 85%] Built target mp_transports
[ 85%] Built target snort
[ 85%] Built target api_options
[ 85%] Built target snort_api
[ 85%] Built target u2boat
[ 85%] Built target u2spewfoo
[ 87%] Built target rule_states
[ 90%] Built target config_states
[ 91%] Built target conversion_data
[ 92%] Built target data_types
[ 92%] Built target snort2lua_helpers
[ 94%] Built target keyword_states
[ 95%] Built target output_states
[ 98%] Built target preprocessor_states
[100%] Built target snort2lua
[100%] Built target show_flows
[100%] Built target daq_file
[100%] Built target daq_hext





──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ snort --daq-list
Available DAQ modules:
afpacket(v7): live inline multi unpriv
 Variables:
  buffer_size_mb <arg> - Packet buffer space to allocate in megabytes
  debug - Enable debugging output to stdout
  fanout_type <arg> - Fanout loadbalancing method
  fanout_flag <arg> - Fanout loadbalancing option
  use_tx_ring - Use memory-mapped TX ring
bpf(v1): inline unpriv wrapper
dump(v5): inline unpriv wrapper
 Variables:
  file <arg> - PCAP filename to output transmitted packets to (default: inline-out.pcap)
  output <arg> - Set to none to prevent output from being written to file (deprecated)
  dump-rx [arg] - Also dump received packets to their own PCAP file (default: inline-in.pcap)
fst(v1): unpriv wrapper
 Variables:
  no_binding_verdicts - Disables enforcement of binding verdicts
  enable_meta_ack - Enables support for filtering bare TCP acks
  ignore_checksums - Ignore bad checksums while decoding
gwlb(v1): inline unpriv wrapper
nfq(v8): live inline multi
 Variables:
  debug - Enable debugging output to stdout
  fail_open - Allow the kernel to bypass the netfilter queue when it is full
  queue_maxlen <arg> - Maximum queue length (default: 1024)
pcap(v4): readback live multi unpriv
 Variables:
  buffer_size <arg> - Packet buffer space to allocate in bytes
  no_promiscuous - Disables opening the interface in promiscuous mode
  no_immediate - Disables immediate mode for traffic capture (may cause unbounded blocking)
  readback_timeout - Return timeout receive status in file readback mode
savefile(v1): readback multi unpriv
trace(v1): inline unpriv wrapper
 Variables:
  file <arg> - Filename to write text traces to (default: inline-out.txt)





  ──(kali㉿kali)-[~]
└─$ sudo apt update                
[sudo] password for kali: 
Get:1 http://kali.download/kali kali-rolling InRelease [34.0 kB]
Get:2 http://kali.download/kali kali-rolling/main amd64 Packages [21.4 MB]
Get:3 http://kali.download/kali kali-rolling/main amd64 Contents (deb) [53.4 MB]
Get:4 http://kali.download/kali kali-rolling/contrib amd64 Packages [105 kB]
Get:5 http://kali.download/kali kali-rolling/contrib amd64 Contents (deb) [190 kB]
Get:6 http://kali.download/kali kali-rolling/non-free-firmware amd64 Packages [15.8 kB]
Get:7 http://kali.download/kali kali-rolling/non-free-firmware amd64 Contents (deb) [40.5 kB]
Fetched 75.2 MB in 2min 33s (492 kB/s)                                      
37 packages can be upgraded. Run 'apt list --upgradable' to see them.
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo apt upgrade
Error: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo dpkg --configure -a
Setting up libatk-bridge2.0-0t64:amd64 (2.61.0-1)…
Setting up php8.4-cli (8.4.23-1)…
Setting up udisks2 (2.11.1-2)…
Setting up python3-flask-kvsession (0.6.4-0kali2)…
Setting up bundler (4.0.15-2)…
Setting up mariadb-client (1:11.8.8-1)…
Setting up libapache2-mod-php8.4 (8.4.23-1)…
libapache2-mod-php8.4: not switching MPM - already enabled
Setting up llvm-21 (1:21.1.8-7+b3)…
Setting up python3-twisted (26.4.0-4)…
Setting up python3-requests (2.32.5+dfsg-2)…
Setting up python3-flask-socketio (5.6.1-0.1)…
Setting up dnsrecon (1.6.0-1)…
Setting up php8.4 (8.4.23-1)…
Setting up libdrm2:amd64 (2.4.134-3)…
Setting up ghp-import (2.1.0-4)…
Setting up libva-drm2:amd64 (2.24.0-1)…
Setting up at-spi2-core (2.61.0-1)…
Setting up ipython3 (9.11.0-2)…
Setting up mariadb-server-core (1:11.8.8-1)…
Setting up python3-paramiko (4.0.0-3)…
Setting up clang-21 (1:21.1.8-7+b3)…
Setting up libva-x11-2:amd64 (2.24.0-1)…
Setting up liblilv-0-0:amd64 (0.28.0-2)…
Setting up libdrm-amdgpu1:amd64 (2.4.134-3)…
Setting up mesa-vulkan-drivers:amd64 (26.1.4-1)…
Setting up libdrm-nouveau2:amd64 (2.4.134-3)…
Setting up llvm-21-dev (1:21.1.8-7+b3)…
Setting up python3-pyexploitdb (0.3.35-0kali1)…
Setting up clang-tools-21 (1:21.1.8-7+b3)…
Setting up mariadb-plugin-provider-lz4 (1:11.8.8-1)…
Setting up libavutil60:amd64 (7:8.1.2-2+b1)…
Setting up libdrm-radeon1:amd64 (2.4.134-3)…
Setting up mariadb-plugin-provider-snappy (1:11.8.8-1)…
Setting up libdrm-intel1:amd64 (2.4.134-3)…
Setting up mariadb-server (1:11.8.8-1)…
Installing new version of config file /etc/mysql/debian-start…
Installing new version of config file /etc/mysql/mariadb.conf.d/50-server.cnf…
Created /etc/mysql/mariadb.conf.d/99-legacy-datadir.cnf for MariaDB to continue using /var/lib/mysql on upgrade.
mariadb.service is a disabled or a static unit not running, not starting it.
Setting up libgstreamer-plugins-bad1.0-0:amd64 (1.28.4-1+b1)…
Setting up mariadb-plugin-provider-bzip2 (1:11.8.8-1)…
Setting up mariadb-plugin-provider-lzma (1:11.8.8-1)…
Setting up libspa-0.2-modules:amd64 (1.6.8-1)…
Setting up libswscale9:amd64 (7:8.1.2-2+b1)…
Setting up gstreamer1.0-plugins-bad:amd64 (1.28.4-1+b1)…
Setting up faraday (5.22.0-0kali1)…
faraday.service is a disabled or a static unit not running, not starting it.
Setting up set (8.0.3+git20260604-0kali1)…
Setting up libswresample6:amd64 (7:8.1.2-2+b1)…
Setting up libspa-0.2-bluetooth:amd64 (1.6.8-1)…
Setting up mariadb-plugin-provider-lzo (1:11.8.8-1)…
Setting up libpipewire-0.3-0t64:amd64 (1.6.8-1)…
Setting up mesa-libgallium:amd64 (26.1.4-1)…
Setting up libgbm1:amd64 (26.1.4-1)…
Setting up mariadb-server-compat (1:11.8.8-1)…
Setting up libgl1-mesa-dri:amd64 (26.1.4-1)…
Setting up libsdl3-0:amd64 (3.4.12+ds-1)…
Setting up libpipewire-0.3-modules:amd64 (1.6.8-1)…
Setting up libegl-mesa0:amd64 (26.1.4-1)…
Setting up libavcodec62:amd64 (7:8.1.2-2+b1)…
Setting up chromium (150.0.7871.114-1)…
Setting up libglx-mesa0:amd64 (26.1.4-1)…
Setting up libavformat62:amd64 (7:8.1.2-2+b1)…
Setting up chromium-driver (150.0.7871.114-1)…
Setting up pipewire-bin (1.6.8-1)…
Setting up libavfilter11:amd64 (7:8.1.2-2+b1)…
Setting up pipewire:amd64 (1.6.8-1)…
Setting up pipewire-pulse (1.6.8-1)…
Setting up libheif-plugin-libde265:amd64 (1.21.2-4+b1)…
Setting up pyinstaller (6.19.0+ds-2)…
Setting up libheif-plugin-dav1d:amd64 (1.21.2-4+b1)…
Setting up powershell-empire (6.6.0-0kali1)…
Installing new version of config file /etc/powershell-empire/server/config.yaml…
powershell-empire.service is a disabled or a static unit not running, not starting it.
Setting up libheif1:amd64 (1.21.2-4+b1)…
Setting up pyinstaller-hooks-contrib (2026.6-1)…
Setting up python3-pyinstaller (6.19.0+ds-2)…
Setting up libmagickcore-7.q16-10:amd64 (8:7.1.2.27+dfsg1-1)…
Setting up libmagickwand-7.q16-10:amd64 (8:7.1.2.27+dfsg1-1)…
Setting up libheif-plugin-x265:amd64 (1.21.2-4+b1)…
Setting up libheif-plugin-aomenc:amd64 (1.21.2-4+b1)…
Setting up libmagickcore-7.q16-10-extra:amd64 (8:7.1.2.27+dfsg1-1)…
Setting up imagemagick-7.q16 (8:7.1.2.27+dfsg1-1)…
Setting up imagemagick (8:7.1.2.27+dfsg1-1)…
Processing triggers for sgml-base (1.31+nmu1)…
Processing triggers for debianutils (5.23.2)…
Processing triggers for base-files (1:2026.3.0)…
Processing triggers for wordlists (2026.2.0)…
Processing triggers for mailcap (3.77)…
Processing triggers for kali-menu (2026.3.2)…
Processing triggers for desktop-file-utils (0.28-1)…
Processing triggers for initramfs-tools (0.151)…
update-initramfs: Generating /boot/initrd.img-7.0.12+kali-amd64
Processing triggers for hicolor-icon-theme (0.18-2)…
Processing triggers for doc-base (0.11.2)…
Processing 3 changed doc-base files...
Processing triggers for libc-bin (2.42-16)…
Processing triggers for systemd (261.1-2)…
Processing triggers for man-db (2.13.1-1)…
Processing triggers for libglib2.0-0t64:amd64 (2.88.2-1)…
Processing triggers for dbus (1.16.2-5+b1)…
Processing triggers for shared-mime-info (2.4-5+b3)…
Processing triggers for php8.4-cli (8.4.23-1)…
Processing triggers for libapache2-mod-php8.4 (8.4.23-1)…
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo apt upgrade        
The following package was automatically installed and is no longer required:
  libx265-215
Use 'sudo apt autoremove' to remove it.

Upgrading:
  arping               libtss2-esys-3.0.2-0t64
  dirmngr              libtss2-mu-4.0.1-0t64                                 
  distro-info-data     libtss2-rc0t64                                        
  firmware-sof-signed  libtss2-sys1t64                                       
  gnupg                libtss2-tcti-cmd0t64                                  
  gnupg-l10n           libtss2-tcti-device0t64                               
  gnupg-utils          libtss2-tcti-libtpms0t64                              
  gpg                  libtss2-tcti-mssim0t64                                
  gpg-agent            libtss2-tcti-spi-helper0t64                           
  gpg-wks-client       libtss2-tcti-swtpm0t64                                
  gpgconf              libtss2-tctildr0t64                                   
  gpgsm                libx264-165                                           
  gpgv                 p11-kit                                               
  libjsoncpp26         p11-kit-modules                                       
  libp11-kit0          python3-httpx                                         
  libpsl5t64           python3-jq                                            
  libselinux1          python3-urllib3                                       
  libsemanage-common   tpm-udev                                              
  libsemanage2                                                               
                                                                             
Installing dependencies:
  selinux-utils
                                                                             
Summary:
  Upgrading: 37, Installing: 1, Removing: 0, Not Upgrading: 0
  Download size: 8,633 kB
  Space needed: 5,943 kB / 57.2 GB available

Continue? [Y/n] Y
Get:1 http://kali.download/kali kali-rolling/non-free-firmware amd64 firmware-sof-signed all 2025.12.2-2 [2,115 kB]
Get:2 http://kali.download/kali kali-rolling/main amd64 libselinux1 amd64 3.11-2 [87.3 kB]
Get:3 http://kali.download/kali kali-rolling/main amd64 libsemanage-common all 3.11-1 [7,148 B]
Get:4 http://kali.download/kali kali-rolling/main amd64 libsemanage2 amd64 3.11-1 [93.2 kB]
Get:5 http://kali.download/kali kali-rolling/main amd64 arping amd64 2.29-1 [34.7 kB]
Get:6 http://kali.download/kali kali-rolling/main amd64 gnupg-utils amd64 2.4.9-7 [192 kB]
Get:7 http://kali.download/kali kali-rolling/main amd64 gpg-wks-client amd64 2.4.9-7 [106 kB]
Get:8 http://kali.download/kali kali-rolling/main amd64 dirmngr amd64 2.4.9-7 [382 kB]
Get:9 http://kali.download/kali kali-rolling/main amd64 gpg-agent amd64 2.4.9-7 [270 kB]
Get:10 http://kali.download/kali kali-rolling/main amd64 gpg amd64 2.4.9-7 [636 kB]
Get:11 http://kali.download/kali kali-rolling/main amd64 gpgconf amd64 2.4.9-7 [126 kB]
Get:12 http://kali.download/kali kali-rolling/main amd64 gnupg all 2.4.9-7 [415 kB]
Get:13 http://kali.download/kali kali-rolling/main amd64 gpgsm amd64 2.4.9-7 [274 kB]
Get:14 http://kali.download/kali kali-rolling/main amd64 gnupg-l10n all 2.4.9-7 [748 kB]
Get:15 http://kali.download/kali kali-rolling/main amd64 distro-info-data all 0.72-1 [6,088 B]
Get:16 http://kali.download/kali kali-rolling/main amd64 gpgv amd64 2.4.9-7 [240 kB]
Get:17 http://kali.download/kali kali-rolling/main amd64 libjsoncpp26 amd64 1.9.8-2 [87.5 kB]
Get:18 http://kali.download/kali kali-rolling/main amd64 p11-kit-modules amd64 0.26.4-1 [313 kB]
Get:19 http://kali.download/kali kali-rolling/main amd64 libp11-kit0 amd64 0.26.4-1 [471 kB]
Get:20 http://kali.download/kali kali-rolling/main amd64 libpsl5t64 amd64 0.23.0-1 [60.8 kB]
Get:21 http://kali.download/kali kali-rolling/main amd64 libtss2-mu-4.0.1-0t64 amd64 4.1.3-7 [77.5 kB]
Get:22 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-cmd0t64 amd64 4.1.3-7 [34.4 kB]
Get:23 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-device0t64 amd64 4.1.3-7 [35.7 kB]
Get:24 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-mssim0t64 amd64 4.1.3-7 [35.8 kB]
Get:25 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-swtpm0t64 amd64 4.1.3-7 [35.9 kB]
Get:26 http://kali.download/kali kali-rolling/main amd64 libtss2-sys1t64 amd64 4.1.3-7 [55.5 kB]
Get:27 http://kali.download/kali kali-rolling/main amd64 libtss2-esys-3.0.2-0t64 amd64 4.1.3-7 [172 kB]
Get:28 http://kali.download/kali kali-rolling/main amd64 libtss2-rc0t64 amd64 4.1.3-7 [31.1 kB]
Get:29 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-libtpms0t64 amd64 4.1.3-7 [34.7 kB]
Get:30 http://kali.download/kali kali-rolling/main amd64 libtss2-tcti-spi-helper0t64 amd64 4.1.3-7 [34.8 kB]
Get:31 http://kali.download/kali kali-rolling/main amd64 libtss2-tctildr0t64 amd64 4.1.3-7 [35.1 kB]
Get:32 http://http.kali.org/kali kali-rolling/main amd64 libx264-165 amd64 2:0.165.3223+git20250910.0480cb0-1 [555 kB]
Get:33 http://kali.download/kali kali-rolling/main amd64 p11-kit amd64 0.26.4-1 [443 kB]
Get:34 http://kali.download/kali kali-rolling/main amd64 python3-httpx all 0.28.1-1.1 [75.1 kB]
Get:35 http://kali.download/kali kali-rolling/main amd64 python3-jq amd64 1.12.0-1 [93.3 kB]
Get:36 http://kali.download/kali kali-rolling/main amd64 python3-urllib3 all 2.7.0-2 [119 kB]
Get:37 http://kali.download/kali kali-rolling/main amd64 selinux-utils amd64 3.11-2 [73.8 kB]
Get:38 http://kali.download/kali kali-rolling/main amd64 tpm-udev all 4.1.3-7 [27.5 kB]
Fetched 8,633 kB in 23s (373 kB/s)                                          
Extracting templates from packages: 100%
(Reading database… 433655 files and directories currently installed.)
Preparing to unpack …/firmware-sof-signed_2025.12.2-2_all.deb…
Unpacking firmware-sof-signed (2025.12.2-2) over (2025.05.1-1)…
Preparing to unpack …/libselinux1_3.11-2_amd64.deb…
Unpacking libselinux1:amd64 (3.11-2) over (3.10-1)…
Setting up libselinux1:amd64 (3.11-2)…
(Reading database… 433724 files and directories currently installed.)
Preparing to unpack …/libsemanage-common_3.11-1_all.deb…
Unpacking libsemanage-common (3.11-1) over (3.10-1)…
Setting up libsemanage-common (3.11-1)…
(Reading database… 433724 files and directories currently installed.)
Preparing to unpack …/libsemanage2_3.11-1_amd64.deb…
Unpacking libsemanage2:amd64 (3.11-1) over (3.10-1)…
Setting up libsemanage2:amd64 (3.11-1)…
(Reading database… 433724 files and directories currently installed.)
Preparing to unpack …/00-arping_2.29-1_amd64.deb…
Unpacking arping (2.29-1) over (2.28-1)…
Preparing to unpack …/01-gnupg-utils_2.4.9-7_amd64.deb…
Unpacking gnupg-utils (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/02-gpg-wks-client_2.4.9-7_amd64.deb…
Unpacking gpg-wks-client (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/03-dirmngr_2.4.9-7_amd64.deb…
Unpacking dirmngr (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/04-gpg-agent_2.4.9-7_amd64.deb…
Unpacking gpg-agent (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/05-gpg_2.4.9-7_amd64.deb…
Unpacking gpg (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/06-gpgconf_2.4.9-7_amd64.deb…
Unpacking gpgconf (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/07-gnupg_2.4.9-7_all.deb…
Unpacking gnupg (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/08-gpgsm_2.4.9-7_amd64.deb…
Unpacking gpgsm (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/09-gnupg-l10n_2.4.9-7_all.deb…
Unpacking gnupg-l10n (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/10-distro-info-data_0.72-1_all.deb…
Unpacking distro-info-data (0.72-1) over (0.71-1)…
Preparing to unpack …/11-gpgv_2.4.9-7_amd64.deb…
Unpacking gpgv (2.4.9-7) over (2.4.9-5)…
Preparing to unpack …/12-libjsoncpp26_1.9.8-2_amd64.deb…
Unpacking libjsoncpp26:amd64 (1.9.8-2) over (1.9.8-1)…
Preparing to unpack …/13-p11-kit-modules_0.26.4-1_amd64.deb…
Unpacking p11-kit-modules:amd64 (0.26.4-1) over (0.26.2-3)…
Preparing to unpack …/14-libp11-kit0_0.26.4-1_amd64.deb…
Unpacking libp11-kit0:amd64 (0.26.4-1) over (0.26.2-3)…
Preparing to unpack …/15-libpsl5t64_0.23.0-1_amd64.deb…
Unpacking libpsl5t64:amd64 (0.23.0-1) over (0.22.0-1)…
Preparing to unpack …/16-libtss2-mu-4.0.1-0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-mu-4.0.1-0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/17-libtss2-tcti-cmd0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-cmd0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/18-libtss2-tcti-device0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-device0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/19-libtss2-tcti-mssim0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-mssim0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/20-libtss2-tcti-swtpm0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-swtpm0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/21-libtss2-sys1t64_4.1.3-7_amd64.deb…
Unpacking libtss2-sys1t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/22-libtss2-esys-3.0.2-0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-esys-3.0.2-0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/23-libtss2-rc0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-rc0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/24-libtss2-tcti-libtpms0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-libtpms0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/25-libtss2-tcti-spi-helper0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tcti-spi-helper0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/26-libtss2-tctildr0t64_4.1.3-7_amd64.deb…
Unpacking libtss2-tctildr0t64:amd64 (4.1.3-7) over (4.1.3-6)…
Preparing to unpack …/27-libx264-165_2%3a0.165.3223+git20250910.0480cb0-1_amd64.deb…
Unpacking libx264-165:amd64 (2:0.165.3223+git20250910.0480cb0-1) over (2:0.165.3222+gitb35605ac-3+b2)…
Preparing to unpack …/28-p11-kit_0.26.4-1_amd64.deb…
Unpacking p11-kit (0.26.4-1) over (0.26.2-3)…
Preparing to unpack …/29-python3-httpx_0.28.1-1.1_all.deb…
Unpacking python3-httpx (0.28.1-1.1) over (0.28.1-1)…
Preparing to unpack …/30-python3-jq_1.12.0-1_amd64.deb…
Unpacking python3-jq (1.12.0-1) over (1.11.0-2)…
Preparing to unpack …/31-python3-urllib3_2.7.0-2_all.deb…
Unpacking python3-urllib3 (2.7.0-2) over (2.7.0-1)…
Selecting previously unselected package selinux-utils.
Preparing to unpack …/32-selinux-utils_3.11-2_amd64.deb…
Unpacking selinux-utils (3.11-2)…
Preparing to unpack …/33-tpm-udev_4.1.3-7_all.deb…
Unpacking tpm-udev (4.1.3-7) over (4.1.3-6)…
Setting up selinux-utils (3.11-2)…
Setting up tpm-udev (4.1.3-7)…
Setting up python3-jq (1.12.0-1)…
Setting up arping (2.29-1)…
Setting up libx264-165:amd64 (2:0.165.3223+git20250910.0480cb0-1)…
Setting up distro-info-data (0.72-1)…
Setting up libtss2-rc0t64:amd64 (4.1.3-7)…
Setting up firmware-sof-signed (2025.12.2-2)…
Setting up libtss2-mu-4.0.1-0t64:amd64 (4.1.3-7)…
Setting up libpsl5t64:amd64 (0.23.0-1)…
Setting up libtss2-tcti-libtpms0t64:amd64 (4.1.3-7)…
Setting up python3-httpx (0.28.1-1.1)…
Setting up libtss2-sys1t64:amd64 (4.1.3-7)…
Setting up gnupg-l10n (2.4.9-7)…
Setting up libjsoncpp26:amd64 (1.9.8-2)…
Setting up libp11-kit0:amd64 (0.26.4-1)…
Setting up libtss2-tcti-device0t64:amd64 (4.1.3-7)…
Setting up python3-urllib3 (2.7.0-2)…
Setting up gpgv (2.4.9-7)…
Setting up libtss2-tcti-mssim0t64:amd64 (4.1.3-7)…
Setting up gpgconf (2.4.9-7)…
Setting up libtss2-tcti-cmd0t64:amd64 (4.1.3-7)…
Setting up libtss2-tcti-swtpm0t64:amd64 (4.1.3-7)…
Setting up gpg (2.4.9-7)…
Setting up gnupg-utils (2.4.9-7)…
Setting up libtss2-tcti-spi-helper0t64:amd64 (4.1.3-7)…
Setting up gpg-agent (2.4.9-7)…
Setting up gpgsm (2.4.9-7)…
Setting up libtss2-tctildr0t64:amd64 (4.1.3-7)…
Setting up dirmngr (2.4.9-7)…
Setting up p11-kit-modules:amd64 (0.26.4-1)…
Setting up libtss2-esys-3.0.2-0t64:amd64 (4.1.3-7)…
Setting up gnupg (2.4.9-7)…
Setting up p11-kit (0.26.4-1)…
Setting up gpg-wks-client (2.4.9-7)…
Processing triggers for man-db (2.13.1-1)…
Processing triggers for kali-menu (2026.3.2)…
Processing triggers for libc-bin (2.42-16)…







──(kali㉿kali)-[~]
└─$ cd ~/snort_src
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ ls                                  
snort3
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ git clone https://github.com/snort3/libdaq.git daq
Cloning into 'daq'...
remote: Enumerating objects: 2691, done.
remote: Counting objects: 100% (313/313), done.
remote: Compressing objects: 100% (125/125), done.
remote: Total 2691 (delta 240), reused 212 (delta 188), pack-reused 2378 (from 2)
Receiving objects: 100% (2691/2691), 1.26 MiB | 23.00 KiB/s, done.
Resolving deltas: 100% (1932/1932), done.
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ cd ~/snort_src/daq
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ ./bootstrap
+ autoreconf -ivf --warnings=all
autoreconf: export WARNINGS=all
autoreconf: Entering directory '.'
autoreconf: configure.ac: no obvious need to run autopoint
autoreconf: running: aclocal --force -I m4
autoreconf: configure.ac: tracing
autoreconf: running: libtoolize --copy --force
libtoolize: putting auxiliary files in '.'.
libtoolize: copying file './ltmain.sh'
libtoolize: putting macros in AC_CONFIG_MACRO_DIRS, 'm4'.
libtoolize: copying file 'm4/libtool.m4'
libtoolize: copying file 'm4/ltoptions.m4'
libtoolize: copying file 'm4/ltsugar.m4'
libtoolize: copying file 'm4/ltversion.m4'
libtoolize: copying file 'm4/lt~obsolete.m4'
autoreconf: configure.ac: not using Intltool
autoreconf: configure.ac: not using Gtkdoc
autoreconf: configure.ac: no need to run autopoint (confirmed)
autoreconf: running: aclocal --force -I m4
autoreconf: running: /usr/bin/autoconf --force
configure.ac:27: warning: The macro 'AC_PROG_CC_C99' is obsolete.
configure.ac:27: You should run autoupdate.
./lib/autoconf/c.m4:1788: AC_PROG_CC_C99 is expanded from...
configure.ac:27: the top level
autoreconf: running: /usr/bin/autoheader --force
autoreconf: running: automake --add-missing --copy --force-missing
configure.ac:29: installing './ar-lib'
configure.ac:26: installing './compile'
configure.ac:34: installing './config.guess'
configure.ac:34: installing './config.sub'
configure.ac:19: installing './install-sh'
configure.ac:19: installing './missing'
api/Makefile.am: installing './depcomp'
parallel-tests: installing './test-driver'
autoreconf: configure.ac: not running make: --make not given
autoreconf: Leaving directory '.'
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ ./configure
checking for a BSD-compatible install... /usr/bin/install -c
checking whether sleep supports fractional seconds... yes
checking filesystem timestamp resolution... 0.01
checking whether build environment is sane... yes
checking for a race-free mkdir -p... /usr/bin/mkdir -p
checking for gawk... gawk
checking whether make sets $(MAKE)... yes
checking whether make supports nested variables... yes
checking xargs -n works... yes
checking whether UID '1000' is supported by ustar format... yes
checking whether GID '1000' is supported by ustar format... yes
checking how to create a ustar tar archive... gnutar
checking for gcc... gcc
checking whether the C compiler works... yes
checking for C compiler default output file name... a.out
checking for suffix of executables... 
checking whether we are cross compiling... no
checking for suffix of object files... o
checking whether the compiler supports GNU C... yes
checking whether gcc accepts -g... yes
checking for gcc option to enable C23 features... none needed
checking whether gcc understands -c and -o together... yes
checking whether make supports the include directive... yes (GNU style)
checking dependency style of gcc... gcc3
checking for g++... g++
checking whether the compiler supports GNU C++... yes
checking whether g++ accepts -g... yes
checking dependency style of g++... gcc3
checking for ar... ar
checking the archiver (ar) interface... ar
checking for a sed that does not truncate output... /usr/bin/sed
checking whether g++ supports C++11 features with -std=gnu++11... yes
checking build system type... x86_64-pc-linux-gnu
checking host system type... x86_64-pc-linux-gnu
checking how to print strings... printf
checking for a sed that does not truncate output... (cached) /usr/bin/sed
checking for grep that handles long lines and -e... /usr/bin/grep
checking for egrep... /usr/bin/grep -E
checking for fgrep... /usr/bin/grep -F
checking for ld used by gcc... /usr/bin/x86_64-linux-gnu-ld
checking if the linker (/usr/bin/x86_64-linux-gnu-ld) is GNU ld... yes
checking for BSD- or MS-compatible name lister (nm)... /usr/bin/nm -B
checking the name lister (/usr/bin/nm -B) interface... BSD nm
checking whether ln -s works... yes
checking the maximum length of command line arguments... 1572864
checking how to convert x86_64-pc-linux-gnu file names to x86_64-pc-linux-gnu format... func_convert_file_noop
checking how to convert x86_64-pc-linux-gnu file names to toolchain format... func_convert_file_noop
checking for /usr/bin/x86_64-linux-gnu-ld option to reload object files... -r
checking for file... file
checking for objdump... objdump
checking how to recognize dependent libraries... pass_all
checking for dlltool... no
checking how to associate runtime and link libraries... printf %s\n
checking for ranlib... ranlib
checking for archiver @FILE support... @
checking for strip... strip
checking command to parse /usr/bin/nm -B output from gcc object... ok
checking for sysroot... no
checking for a working dd... /usr/bin/dd
checking how to truncate binary pipes... /usr/bin/dd bs=4096 count=1
checking for mt... mt
checking if mt is a manifest tool... no
checking for stdio.h... yes
checking for stdlib.h... yes
checking for string.h... yes
checking for inttypes.h... yes
checking for stdint.h... yes
checking for strings.h... yes
checking for sys/stat.h... yes
checking for sys/types.h... yes
checking for unistd.h... yes
checking for sys/param.h... yes
checking for dlfcn.h... yes
checking for objdir... .libs
checking if gcc supports -fno-rtti -fno-exceptions... no
checking for gcc option to produce PIC... -fPIC -DPIC
checking if gcc PIC flag -fPIC -DPIC works... yes
checking if gcc static flag -static works... yes
checking if gcc supports -c -o file.o... yes
checking if gcc supports -c -o file.o... (cached) yes
checking whether the gcc linker (/usr/bin/x86_64-linux-gnu-ld -m elf_x86_64) supports shared libraries... yes
checking whether -lc should be explicitly linked in... no
checking dynamic linker characteristics... GNU/Linux ld.so
checking how to hardcode library paths into programs... immediate
checking whether stripping libraries is possible... yes
checking if libtool supports shared libraries... yes
checking whether to build shared libraries... yes
checking whether to build static libraries... yes
checking how to run the C++ preprocessor... g++ -std=gnu++11 -E
checking for ld used by g++ -std=gnu++11... /usr/bin/x86_64-linux-gnu-ld -m elf_x86_64
checking if the linker (/usr/bin/x86_64-linux-gnu-ld -m elf_x86_64) is GNU ld... yes
checking whether the g++ -std=gnu++11 linker (/usr/bin/x86_64-linux-gnu-ld -m elf_x86_64) supports shared libraries... yes
checking for g++ -std=gnu++11 option to produce PIC... -fPIC -DPIC
checking if g++ -std=gnu++11 PIC flag -fPIC -DPIC works... yes
checking if g++ -std=gnu++11 static flag -static works... yes
checking if g++ -std=gnu++11 supports -c -o file.o... yes
checking if g++ -std=gnu++11 supports -c -o file.o... (cached) yes
checking whether the g++ -std=gnu++11 linker (/usr/bin/x86_64-linux-gnu-ld -m elf_x86_64) supports shared libraries... yes
checking dynamic linker characteristics... (cached) GNU/Linux ld.so
checking how to hardcode library paths into programs... immediate
checking whether the -Werror option is usable... yes
checking for simple visibility declarations... yes
checking how to run the C preprocessor... gcc -E
checking whether C preprocessor accepts -Wall... yes
checking whether C preprocessor accepts -Wmissing-declarations... yes
checking whether C preprocessor accepts -Wpointer-arith... yes
checking whether C preprocessor accepts -Wcast-align... yes
checking whether C preprocessor accepts -Wcast-qual... yes
checking whether C preprocessor accepts -Wformat... yes
checking whether C preprocessor accepts -Wformat-nonliteral... yes
checking whether C preprocessor accepts -Wformat-security... yes
checking whether C preprocessor accepts -Wundef... yes
checking whether C preprocessor accepts -Wwrite-strings... yes
checking whether C preprocessor accepts -Wextra... yes
checking whether C preprocessor accepts -Wsign-compare... yes
checking whether C preprocessor accepts -Wno-unused-parameter... yes
checking whether C preprocessor accepts -fno-strict-aliasing... yes
checking whether C preprocessor accepts -fdiagnostics-show-option... yes
checking whether C preprocessor accepts -Wstrict-prototypes... yes
checking whether C preprocessor accepts -Wmissing-prototypes... yes
checking whether C preprocessor accepts -Wold-style-definition... yes
checking whether C preprocessor accepts -Wnested-externs... yes
checking whether to build with code coverage support... no
checking for pkg-config... /usr/bin/pkg-config
checking pkg-config is at least version 0.9.0... yes
configure: WARNING: No libcmocka-1.0.0 or newer library found, cmocka tests will not be built
checking for pcap.h... yes
checking for pcap_lib_version in -lpcap... yes
checking for linux/if_ether.h... yes
checking for linux/if_packet.h... yes
checking for gcc options to detect undeclared functions... none needed
checking for gcc options to ignore future-version functions... none needed
checking whether PACKET_FANOUT_QM is declared... yes
checking whether PACKET_QDISC_BYPASS is declared... yes
checking whether TP_STATUS_VLAN_TPID_VALID is declared... yes
checking whether IPPROTO_DIVERT is declared... no
checking for net/netmap.h... no
checking for net/netmap_user.h... no
checking whether NETMAP_API is declared... no
checking for linux/netfilter.h... yes
checking for linux/netfilter/nfnetlink_queue.h... yes
checking for libmnl/libmnl.h... no
checking for mnl_socket_open in -lmnl... no
checking for dlopen in -ldl... yes
checking for inttypes.h... (cached) yes
checking for memory.h... yes
checking for netdb.h... yes
checking for netinet/in.h... yes
checking for stdint.h... (cached) yes
checking for stdlib.h... (cached) yes
checking for string.h... (cached) yes
checking for sys/ioctl.h... yes
checking for sys/param.h... (cached) yes
checking for sys/socket.h... yes
checking for sys/time.h... yes
checking for unistd.h... (cached) yes
checking for inline... inline
checking for size_t... yes
checking for uint16_t... yes
checking for uint32_t... yes
checking for uint64_t... yes
checking for uint8_t... yes
checking whether malloc (0) returns nonnull... yes
checking for getpagesize... yes
checking for working mmap... yes
checking for gethostbyname... yes
checking for getpagesize... (cached) yes
checking for memset... yes
checking for munmap... yes
checking for socket... yes
checking for strchr... yes
checking for strcspn... yes
checking for strdup... yes
checking for strerror... yes
checking for strrchr... yes
checking for strstr... yes
checking for strtoul... yes
checking that generated files are newer than configure... done
configure: creating ./config.status
config.status: creating modules/afpacket/libdaq_static_afpacket.pc
config.status: creating modules/bpf/libdaq_static_bpf.pc
config.status: creating modules/dump/libdaq_static_dump.pc
config.status: creating modules/fst/libdaq_static_fst.pc
config.status: creating modules/pcap/libdaq_static_pcap.pc
config.status: creating modules/savefile/libdaq_static_savefile.pc
config.status: creating modules/trace/libdaq_static_trace.pc
config.status: creating modules/gwlb/libdaq_static_gwlb.pc
config.status: creating Makefile
config.status: creating api/daq_version.h
config.status: creating api/Makefile
config.status: creating example/Makefile
config.status: creating modules/Makefile
config.status: creating test/Makefile
config.status: creating libdaq.pc
config.status: creating config.h
config.status: executing depfiles commands
config.status: executing libtool commands

    libdaq 3.0.27

    prefix:         /usr/local
    sysconfdir:     ${prefix}/etc
    libdir:         ${exec_prefix}/lib
    includedir:     ${prefix}/include

    cc:             gcc
    cppflags:       
    am_cppflags:     -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option
    cflags:         -g -O2
    am_cflags:       -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs
    ldflags:        
    am_ldflags:     
    libs:           

    code_coverage_enabled:  no
    code_coverage_cppflags: 
    code_coverage_cflags:   
    code_coverage_ldflags:  

    Build AFPacket DAQ module.. : yes
    Build BPF DAQ module....... : yes
    Build Divert DAQ module.... : no
    Build Dump DAQ module...... : yes
    Build FST DAQ module....... : yes
    Build netmap DAQ module.... : no
    Build NFQ DAQ module....... : no
    Build PCAP DAQ module...... : yes
    Build Savefile DAQ module.. : yes
    Build Trace DAQ module..... : yes
    Build GWLB DAQ module...... : yes

                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ make -j$(nproc)
make  all-recursive
make[1]: Entering directory '/home/kali/snort_src/daq'
Making all in api
make[2]: Entering directory '/home/kali/snort_src/daq/api'
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2 -MT libdaq_la-daq_base.lo -MD -MP -MF .deps/libdaq_la-daq_base.Tpo -c -o libdaq_la-daq_base.lo `test -f 'daq_base.c' || echo './'`daq_base.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_base.lo -MD -MP -MF .deps/libdaq_la-daq_base.Tpo -c daq_base.c  -fPIC -DPIC -o .libs/libdaq_la-daq_base.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_base.lo -MD -MP -MF .deps/libdaq_la-daq_base.Tpo -c daq_base.c -o libdaq_la-daq_base.o >/dev/null 2>&1
mv -f .deps/libdaq_la-daq_base.Tpo .deps/libdaq_la-daq_base.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2 -MT libdaq_la-daq_base_api.lo -MD -MP -MF .deps/libdaq_la-daq_base_api.Tpo -c -o libdaq_la-daq_base_api.lo `test -f 'daq_base_api.c' || echo './'`daq_base_api.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_base_api.lo -MD -MP -MF .deps/libdaq_la-daq_base_api.Tpo -c daq_base_api.c  -fPIC -DPIC -o .libs/libdaq_la-daq_base_api.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_base_api.lo -MD -MP -MF .deps/libdaq_la-daq_base_api.Tpo -c daq_base_api.c -o libdaq_la-daq_base_api.o >/dev/null 2>&1
mv -f .deps/libdaq_la-daq_base_api.Tpo .deps/libdaq_la-daq_base_api.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2 -MT libdaq_la-daq_config.lo -MD -MP -MF .deps/libdaq_la-daq_config.Tpo -c -o libdaq_la-daq_config.lo `test -f 'daq_config.c' || echo './'`daq_config.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_config.lo -MD -MP -MF .deps/libdaq_la-daq_config.Tpo -c daq_config.c  -fPIC -DPIC -o .libs/libdaq_la-daq_config.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_config.lo -MD -MP -MF .deps/libdaq_la-daq_config.Tpo -c daq_config.c -o libdaq_la-daq_config.o >/dev/null 2>&1
mv -f .deps/libdaq_la-daq_config.Tpo .deps/libdaq_la-daq_config.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2 -MT libdaq_la-daq_instance_api_defaults.lo -MD -MP -MF .deps/libdaq_la-daq_instance_api_defaults.Tpo -c -o libdaq_la-daq_instance_api_defaults.lo `test -f 'daq_instance_api_defaults.c' || echo './'`daq_instance_api_defaults.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_instance_api_defaults.lo -MD -MP -MF .deps/libdaq_la-daq_instance_api_defaults.Tpo -c daq_instance_api_defaults.c  -fPIC -DPIC -o .libs/libdaq_la-daq_instance_api_defaults.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_instance_api_defaults.lo -MD -MP -MF .deps/libdaq_la-daq_instance_api_defaults.Tpo -c daq_instance_api_defaults.c -o libdaq_la-daq_instance_api_defaults.o >/dev/null 2>&1
mv -f .deps/libdaq_la-daq_instance_api_defaults.Tpo .deps/libdaq_la-daq_instance_api_defaults.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2 -MT libdaq_la-daq_mod_ops.lo -MD -MP -MF .deps/libdaq_la-daq_mod_ops.Tpo -c -o libdaq_la-daq_mod_ops.lo `test -f 'daq_mod_ops.c' || echo './'`daq_mod_ops.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_mod_ops.lo -MD -MP -MF .deps/libdaq_la-daq_mod_ops.Tpo -c daq_mod_ops.c  -fPIC -DPIC -o .libs/libdaq_la-daq_mod_ops.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT libdaq_la-daq_mod_ops.lo -MD -MP -MF .deps/libdaq_la-daq_mod_ops.Tpo -c daq_mod_ops.c -o libdaq_la-daq_mod_ops.o >/dev/null 2>&1
mv -f .deps/libdaq_la-daq_mod_ops.Tpo .deps/libdaq_la-daq_mod_ops.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs  -g -O2  -version-info 3:0:0  -o libdaq.la -rpath /usr/local/lib libdaq_la-daq_base.lo libdaq_la-daq_base_api.lo libdaq_la-daq_config.lo libdaq_la-daq_instance_api_defaults.lo libdaq_la-daq_mod_ops.lo -ldl 
libtool: link: gcc -shared  -fPIC -DPIC  .libs/libdaq_la-daq_base.o .libs/libdaq_la-daq_base_api.o .libs/libdaq_la-daq_config.o .libs/libdaq_la-daq_instance_api_defaults.o .libs/libdaq_la-daq_mod_ops.o   -ldl  -g -O2   -Wl,-soname -Wl,libdaq.so.3 -o .libs/libdaq.so.3.0.0
libtool: link: (cd ".libs" && rm -f "libdaq.so.3" && ln -s "libdaq.so.3.0.0" "libdaq.so.3")
libtool: link: (cd ".libs" && rm -f "libdaq.so" && ln -s "libdaq.so.3.0.0" "libdaq.so")
libtool: link: ar cr .libs/libdaq.a  libdaq_la-daq_base.o libdaq_la-daq_base_api.o libdaq_la-daq_config.o libdaq_la-daq_instance_api_defaults.o libdaq_la-daq_mod_ops.o
libtool: link: ranlib .libs/libdaq.a
libtool: link: ( cd ".libs" && rm -f "libdaq.la" && ln -s "../libdaq.la" "libdaq.la" )
make[2]: Leaving directory '/home/kali/snort_src/daq/api'
Making all in modules
make[2]: Entering directory '/home/kali/snort_src/daq/modules'
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/libdaq_static_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/libdaq_static_afpacket_la-daq_afpacket.Tpo -c -o afpacket/libdaq_static_afpacket_la-daq_afpacket.lo `test -f 'afpacket/daq_afpacket.c' || echo './'`afpacket/daq_afpacket.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/libdaq_static_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/libdaq_static_afpacket_la-daq_afpacket.Tpo -c afpacket/daq_afpacket.c  -fPIC -DPIC -o afpacket/.libs/libdaq_static_afpacket_la-daq_afpacket.o
afpacket/daq_afpacket.c: In function 'create_packet_pool':
afpacket/daq_afpacket.c:190:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  190 |     pool->pool = calloc(sizeof(AFPacketPktDesc), size);
      |                                ^~~~~~~~~~~~~~~
afpacket/daq_afpacket.c:190:32: note: earlier argument should specify number of elements, later size of each element
afpacket/daq_afpacket.c: In function 'afpacket_daq_set_filter':
afpacket/daq_afpacket.c:1041:5: warning: 'pcap_compile_nopcap' is deprecated: use pcap_open_dead(), pcap_compile() and pcap_close() [-Wdeprecated-declarations]
 1041 |     if (pcap_compile_nopcap(afpc->snaplen, DLT_EN10MB, &fcode, afpc->filter, 1, PCAP_NETMASK_UNKNOWN) == -1)
      |     ^~
In file included from /usr/include/pcap.h:43,
                 from afpacket/daq_afpacket.c:47:
/usr/include/pcap/pcap.h:667:17: note: declared here
  667 | PCAP_API int    pcap_compile_nopcap(int, int, struct bpf_program *,
      |                 ^~~~~~~~~~~~~~~~~~~
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/libdaq_static_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/libdaq_static_afpacket_la-daq_afpacket.Tpo -c afpacket/daq_afpacket.c -o afpacket/libdaq_static_afpacket_la-daq_afpacket.o >/dev/null 2>&1
mv -f afpacket/.deps/libdaq_static_afpacket_la-daq_afpacket.Tpo afpacket/.deps/libdaq_static_afpacket_la-daq_afpacket.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o afpacket/libdaq_static_afpacket.la -rpath /usr/local/lib afpacket/libdaq_static_afpacket_la-daq_afpacket.lo  
libtool: link: ar cr afpacket/.libs/libdaq_static_afpacket.a  afpacket/libdaq_static_afpacket_la-daq_afpacket.o
libtool: link: ranlib afpacket/.libs/libdaq_static_afpacket.a
libtool: link: ( cd "afpacket/.libs" && rm -f "libdaq_static_afpacket.la" && ln -s "../libdaq_static_afpacket.la" "libdaq_static_afpacket.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/libdaq_static_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/libdaq_static_bpf_la-daq_bpf.Tpo -c -o bpf/libdaq_static_bpf_la-daq_bpf.lo `test -f 'bpf/daq_bpf.c' || echo './'`bpf/daq_bpf.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/libdaq_static_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/libdaq_static_bpf_la-daq_bpf.Tpo -c bpf/daq_bpf.c  -fPIC -DPIC -o bpf/.libs/libdaq_static_bpf_la-daq_bpf.o
bpf/daq_bpf.c: In function 'bpf_daq_set_filter':
bpf/daq_bpf.c:131:5: warning: 'pcap_compile_nopcap' is deprecated: use pcap_open_dead(), pcap_compile() and pcap_close() [-Wdeprecated-declarations]
  131 |     if (pcap_compile_nopcap(bc->snaplen, DLT_EN10MB, &fcode, bc->filter, 1, PCAP_NETMASK_UNKNOWN) == -1)
      |     ^~
In file included from /usr/include/pcap.h:43,
                 from bpf/daq_bpf.c:25:
/usr/include/pcap/pcap.h:667:17: note: declared here
  667 | PCAP_API int    pcap_compile_nopcap(int, int, struct bpf_program *,
      |                 ^~~~~~~~~~~~~~~~~~~
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/libdaq_static_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/libdaq_static_bpf_la-daq_bpf.Tpo -c bpf/daq_bpf.c -o bpf/libdaq_static_bpf_la-daq_bpf.o >/dev/null 2>&1
mv -f bpf/.deps/libdaq_static_bpf_la-daq_bpf.Tpo bpf/.deps/libdaq_static_bpf_la-daq_bpf.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o bpf/libdaq_static_bpf.la -rpath /usr/local/lib bpf/libdaq_static_bpf_la-daq_bpf.lo  
libtool: link: ar cr bpf/.libs/libdaq_static_bpf.a  bpf/libdaq_static_bpf_la-daq_bpf.o
libtool: link: ranlib bpf/.libs/libdaq_static_bpf.a
libtool: link: ( cd "bpf/.libs" && rm -f "libdaq_static_bpf.la" && ln -s "../libdaq_static_bpf.la" "libdaq_static_bpf.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/libdaq_static_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/libdaq_static_dump_la-daq_dump.Tpo -c -o dump/libdaq_static_dump_la-daq_dump.lo `test -f 'dump/daq_dump.c' || echo './'`dump/daq_dump.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/libdaq_static_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/libdaq_static_dump_la-daq_dump.Tpo -c dump/daq_dump.c  -fPIC -DPIC -o dump/.libs/libdaq_static_dump_la-daq_dump.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/libdaq_static_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/libdaq_static_dump_la-daq_dump.Tpo -c dump/daq_dump.c -o dump/libdaq_static_dump_la-daq_dump.o >/dev/null 2>&1
mv -f dump/.deps/libdaq_static_dump_la-daq_dump.Tpo dump/.deps/libdaq_static_dump_la-daq_dump.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o dump/libdaq_static_dump.la -rpath /usr/local/lib dump/libdaq_static_dump_la-daq_dump.lo  
libtool: link: ar cr dump/.libs/libdaq_static_dump.a  dump/libdaq_static_dump_la-daq_dump.o
libtool: link: ranlib dump/.libs/libdaq_static_dump.a
libtool: link: ( cd "dump/.libs" && rm -f "libdaq_static_dump.la" && ln -s "../libdaq_static_dump.la" "libdaq_static_dump.la" )
/bin/bash ../libtool  --tag=CXX   --mode=compile g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example   -g -O2 -MT fst/libdaq_static_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-daq_fst.Tpo -c -o fst/libdaq_static_fst_la-daq_fst.lo `test -f 'fst/daq_fst.cc' || echo './'`fst/daq_fst.cc
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -g -O2 -MT fst/libdaq_static_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-daq_fst.Tpo -c fst/daq_fst.cc  -fPIC -DPIC -o fst/.libs/libdaq_static_fst_la-daq_fst.o
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -g -O2 -MT fst/libdaq_static_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-daq_fst.Tpo -c fst/daq_fst.cc -o fst/libdaq_static_fst_la-daq_fst.o >/dev/null 2>&1
mv -f fst/.deps/libdaq_static_fst_la-daq_fst.Tpo fst/.deps/libdaq_static_fst_la-daq_fst.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/libdaq_static_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-PMurHash.Tpo -c -o fst/libdaq_static_fst_la-PMurHash.lo `test -f 'fst/PMurHash.c' || echo './'`fst/PMurHash.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/libdaq_static_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-PMurHash.Tpo -c fst/PMurHash.c  -fPIC -DPIC -o fst/.libs/libdaq_static_fst_la-PMurHash.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/libdaq_static_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/libdaq_static_fst_la-PMurHash.Tpo -c fst/PMurHash.c -o fst/libdaq_static_fst_la-PMurHash.o >/dev/null 2>&1
mv -f fst/.deps/libdaq_static_fst_la-PMurHash.Tpo fst/.deps/libdaq_static_fst_la-PMurHash.Plo
/bin/bash ../libtool  --tag=CXX   --mode=link g++ -std=gnu++11  -g -O2 -static -avoid-version  -o fst/libdaq_static_fst.la -rpath /usr/local/lib fst/libdaq_static_fst_la-daq_fst.lo fst/libdaq_static_fst_la-PMurHash.lo  
libtool: link: ar cr fst/.libs/libdaq_static_fst.a  fst/libdaq_static_fst_la-daq_fst.o fst/libdaq_static_fst_la-PMurHash.o
libtool: link: ranlib fst/.libs/libdaq_static_fst.a
libtool: link: ( cd "fst/.libs" && rm -f "libdaq_static_fst.la" && ln -s "../libdaq_static_fst.la" "libdaq_static_fst.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/libdaq_static_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/libdaq_static_pcap_la-daq_pcap.Tpo -c -o pcap/libdaq_static_pcap_la-daq_pcap.lo `test -f 'pcap/daq_pcap.c' || echo './'`pcap/daq_pcap.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/libdaq_static_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/libdaq_static_pcap_la-daq_pcap.Tpo -c pcap/daq_pcap.c  -fPIC -DPIC -o pcap/.libs/libdaq_static_pcap_la-daq_pcap.o
pcap/daq_pcap.c: In function 'create_packet_pool':
pcap/daq_pcap.c:126:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  126 |     pool->pool = calloc(sizeof(PcapPktDesc), size);
      |                                ^~~~~~~~~~~
pcap/daq_pcap.c:126:32: note: earlier argument should specify number of elements, later size of each element
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/libdaq_static_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/libdaq_static_pcap_la-daq_pcap.Tpo -c pcap/daq_pcap.c -o pcap/libdaq_static_pcap_la-daq_pcap.o >/dev/null 2>&1
mv -f pcap/.deps/libdaq_static_pcap_la-daq_pcap.Tpo pcap/.deps/libdaq_static_pcap_la-daq_pcap.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o pcap/libdaq_static_pcap.la -rpath /usr/local/lib pcap/libdaq_static_pcap_la-daq_pcap.lo  
libtool: link: ar cr pcap/.libs/libdaq_static_pcap.a  pcap/libdaq_static_pcap_la-daq_pcap.o
libtool: link: ranlib pcap/.libs/libdaq_static_pcap.a
libtool: link: ( cd "pcap/.libs" && rm -f "libdaq_static_pcap.la" && ln -s "../libdaq_static_pcap.la" "libdaq_static_pcap.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/libdaq_static_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/libdaq_static_savefile_la-daq_savefile.Tpo -c -o savefile/libdaq_static_savefile_la-daq_savefile.lo `test -f 'savefile/daq_savefile.c' || echo './'`savefile/daq_savefile.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/libdaq_static_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/libdaq_static_savefile_la-daq_savefile.Tpo -c savefile/daq_savefile.c  -fPIC -DPIC -o savefile/.libs/libdaq_static_savefile_la-daq_savefile.o
savefile/daq_savefile.c: In function 'create_message_pool':
savefile/daq_savefile.c:125:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  125 |     pool->pool = calloc(sizeof(SavefileMsgDesc), size);
      |                                ^~~~~~~~~~~~~~~
savefile/daq_savefile.c:125:32: note: earlier argument should specify number of elements, later size of each element
savefile/daq_savefile.c: In function 'savefile_read_message':
savefile/daq_savefile.c:167:43: warning: comparison of integer expressions of different signedness: 'long unsigned int' and 'off_t' {aka 'long int'} [-Wsign-compare]
  167 |     if (sfc->file_offset + sizeof(*sfhdr) > sfc->file_size)
      |                                           ^
savefile/daq_savefile.c: In function 'savefile_daq_start':
savefile/daq_savefile.c:315:24: warning: comparison of integer expressions of different signedness: 'off_t' {aka 'long int'} and 'long unsigned int' [-Wsign-compare]
  315 |     if (sfc->file_size < sizeof(struct pcap_file_header))
      |                        ^
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/libdaq_static_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/libdaq_static_savefile_la-daq_savefile.Tpo -c savefile/daq_savefile.c -o savefile/libdaq_static_savefile_la-daq_savefile.o >/dev/null 2>&1
mv -f savefile/.deps/libdaq_static_savefile_la-daq_savefile.Tpo savefile/.deps/libdaq_static_savefile_la-daq_savefile.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o savefile/libdaq_static_savefile.la -rpath /usr/local/lib savefile/libdaq_static_savefile_la-daq_savefile.lo  
libtool: link: ar cr savefile/.libs/libdaq_static_savefile.a  savefile/libdaq_static_savefile_la-daq_savefile.o
libtool: link: ranlib savefile/.libs/libdaq_static_savefile.a
libtool: link: ( cd "savefile/.libs" && rm -f "libdaq_static_savefile.la" && ln -s "../libdaq_static_savefile.la" "libdaq_static_savefile.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/libdaq_static_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/libdaq_static_trace_la-daq_trace.Tpo -c -o trace/libdaq_static_trace_la-daq_trace.lo `test -f 'trace/daq_trace.c' || echo './'`trace/daq_trace.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/libdaq_static_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/libdaq_static_trace_la-daq_trace.Tpo -c trace/daq_trace.c  -fPIC -DPIC -o trace/.libs/libdaq_static_trace_la-daq_trace.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/libdaq_static_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/libdaq_static_trace_la-daq_trace.Tpo -c trace/daq_trace.c -o trace/libdaq_static_trace_la-daq_trace.o >/dev/null 2>&1
mv -f trace/.deps/libdaq_static_trace_la-daq_trace.Tpo trace/.deps/libdaq_static_trace_la-daq_trace.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -static -avoid-version  -o trace/libdaq_static_trace.la -rpath /usr/local/lib trace/libdaq_static_trace_la-daq_trace.lo  
libtool: link: ar cr trace/.libs/libdaq_static_trace.a  trace/libdaq_static_trace_la-daq_trace.o
libtool: link: ranlib trace/.libs/libdaq_static_trace.a
libtool: link: ( cd "trace/.libs" && rm -f "libdaq_static_trace.la" && ln -s "../libdaq_static_trace.la" "libdaq_static_trace.la" )
/bin/bash ../libtool  --tag=CXX   --mode=compile g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api   -g -O2 -MT gwlb/libdaq_static_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/libdaq_static_gwlb_la-daq_gwlb.Tpo -c -o gwlb/libdaq_static_gwlb_la-daq_gwlb.lo `test -f 'gwlb/daq_gwlb.cc' || echo './'`gwlb/daq_gwlb.cc
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -g -O2 -MT gwlb/libdaq_static_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/libdaq_static_gwlb_la-daq_gwlb.Tpo -c gwlb/daq_gwlb.cc  -fPIC -DPIC -o gwlb/.libs/libdaq_static_gwlb_la-daq_gwlb.o
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -g -O2 -MT gwlb/libdaq_static_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/libdaq_static_gwlb_la-daq_gwlb.Tpo -c gwlb/daq_gwlb.cc -o gwlb/libdaq_static_gwlb_la-daq_gwlb.o >/dev/null 2>&1
mv -f gwlb/.deps/libdaq_static_gwlb_la-daq_gwlb.Tpo gwlb/.deps/libdaq_static_gwlb_la-daq_gwlb.Plo
/bin/bash ../libtool  --tag=CXX   --mode=link g++ -std=gnu++11  -g -O2 -static -avoid-version  -o gwlb/libdaq_static_gwlb.la -rpath /usr/local/lib gwlb/libdaq_static_gwlb_la-daq_gwlb.lo  
libtool: link: ar cr gwlb/.libs/libdaq_static_gwlb.a  gwlb/libdaq_static_gwlb_la-daq_gwlb.o
libtool: link: ranlib gwlb/.libs/libdaq_static_gwlb.a
libtool: link: ( cd "gwlb/.libs" && rm -f "libdaq_static_gwlb.la" && ln -s "../libdaq_static_gwlb.la" "libdaq_static_gwlb.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/daq_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/daq_afpacket_la-daq_afpacket.Tpo -c -o afpacket/daq_afpacket_la-daq_afpacket.lo `test -f 'afpacket/daq_afpacket.c' || echo './'`afpacket/daq_afpacket.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/daq_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/daq_afpacket_la-daq_afpacket.Tpo -c afpacket/daq_afpacket.c  -fPIC -DPIC -o afpacket/.libs/daq_afpacket_la-daq_afpacket.o
afpacket/daq_afpacket.c: In function 'create_packet_pool':
afpacket/daq_afpacket.c:190:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  190 |     pool->pool = calloc(sizeof(AFPacketPktDesc), size);
      |                                ^~~~~~~~~~~~~~~
afpacket/daq_afpacket.c:190:32: note: earlier argument should specify number of elements, later size of each element
afpacket/daq_afpacket.c: In function 'afpacket_daq_set_filter':
afpacket/daq_afpacket.c:1041:5: warning: 'pcap_compile_nopcap' is deprecated: use pcap_open_dead(), pcap_compile() and pcap_close() [-Wdeprecated-declarations]
 1041 |     if (pcap_compile_nopcap(afpc->snaplen, DLT_EN10MB, &fcode, afpc->filter, 1, PCAP_NETMASK_UNKNOWN) == -1)
      |     ^~
In file included from /usr/include/pcap.h:43,
                 from afpacket/daq_afpacket.c:47:
/usr/include/pcap/pcap.h:667:17: note: declared here
  667 | PCAP_API int    pcap_compile_nopcap(int, int, struct bpf_program *,
      |                 ^~~~~~~~~~~~~~~~~~~
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT afpacket/daq_afpacket_la-daq_afpacket.lo -MD -MP -MF afpacket/.deps/daq_afpacket_la-daq_afpacket.Tpo -c afpacket/daq_afpacket.c -o afpacket/daq_afpacket_la-daq_afpacket.o >/dev/null 2>&1
mv -f afpacket/.deps/daq_afpacket_la-daq_afpacket.Tpo afpacket/.deps/daq_afpacket_la-daq_afpacket.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared   -o afpacket/daq_afpacket.la -rpath /usr/local/lib/daq afpacket/daq_afpacket_la-daq_afpacket.lo -lpcap -lpthread 
libtool: link: gcc -shared  -fPIC -DPIC  afpacket/.libs/daq_afpacket_la-daq_afpacket.o   -lpcap -lpthread  -g -O2   -Wl,-soname -Wl,daq_afpacket.so -o afpacket/.libs/daq_afpacket.so
libtool: link: ( cd "afpacket/.libs" && rm -f "daq_afpacket.la" && ln -s "../daq_afpacket.la" "daq_afpacket.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/daq_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/daq_bpf_la-daq_bpf.Tpo -c -o bpf/daq_bpf_la-daq_bpf.lo `test -f 'bpf/daq_bpf.c' || echo './'`bpf/daq_bpf.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/daq_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/daq_bpf_la-daq_bpf.Tpo -c bpf/daq_bpf.c  -fPIC -DPIC -o bpf/.libs/daq_bpf_la-daq_bpf.o
bpf/daq_bpf.c: In function 'bpf_daq_set_filter':
bpf/daq_bpf.c:131:5: warning: 'pcap_compile_nopcap' is deprecated: use pcap_open_dead(), pcap_compile() and pcap_close() [-Wdeprecated-declarations]
  131 |     if (pcap_compile_nopcap(bc->snaplen, DLT_EN10MB, &fcode, bc->filter, 1, PCAP_NETMASK_UNKNOWN) == -1)
      |     ^~
In file included from /usr/include/pcap.h:43,
                 from bpf/daq_bpf.c:25:
/usr/include/pcap/pcap.h:667:17: note: declared here
  667 | PCAP_API int    pcap_compile_nopcap(int, int, struct bpf_program *,
      |                 ^~~~~~~~~~~~~~~~~~~
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT bpf/daq_bpf_la-daq_bpf.lo -MD -MP -MF bpf/.deps/daq_bpf_la-daq_bpf.Tpo -c bpf/daq_bpf.c -o bpf/daq_bpf_la-daq_bpf.o >/dev/null 2>&1
mv -f bpf/.deps/daq_bpf_la-daq_bpf.Tpo bpf/.deps/daq_bpf_la-daq_bpf.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared   -o bpf/daq_bpf.la -rpath /usr/local/lib/daq bpf/daq_bpf_la-daq_bpf.lo -lpcap -lpthread 
libtool: link: gcc -shared  -fPIC -DPIC  bpf/.libs/daq_bpf_la-daq_bpf.o   -lpcap -lpthread  -g -O2   -Wl,-soname -Wl,daq_bpf.so -o bpf/.libs/daq_bpf.so
libtool: link: ( cd "bpf/.libs" && rm -f "daq_bpf.la" && ln -s "../daq_bpf.la" "daq_bpf.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/daq_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/daq_dump_la-daq_dump.Tpo -c -o dump/daq_dump_la-daq_dump.lo `test -f 'dump/daq_dump.c' || echo './'`dump/daq_dump.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/daq_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/daq_dump_la-daq_dump.Tpo -c dump/daq_dump.c  -fPIC -DPIC -o dump/.libs/daq_dump_la-daq_dump.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT dump/daq_dump_la-daq_dump.lo -MD -MP -MF dump/.deps/daq_dump_la-daq_dump.Tpo -c dump/daq_dump.c -o dump/daq_dump_la-daq_dump.o >/dev/null 2>&1
mv -f dump/.deps/daq_dump_la-daq_dump.Tpo dump/.deps/daq_dump_la-daq_dump.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared   -o dump/daq_dump.la -rpath /usr/local/lib/daq dump/daq_dump_la-daq_dump.lo -lpcap 
libtool: link: gcc -shared  -fPIC -DPIC  dump/.libs/daq_dump_la-daq_dump.o   -lpcap  -g -O2   -Wl,-soname -Wl,daq_dump.so -o dump/.libs/daq_dump.so
libtool: link: ( cd "dump/.libs" && rm -f "daq_dump.la" && ln -s "../daq_dump.la" "daq_dump.la" )
/bin/bash ../libtool  --tag=CXX   --mode=compile g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO   -g -O2 -MT fst/daq_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/daq_fst_la-daq_fst.Tpo -c -o fst/daq_fst_la-daq_fst.lo `test -f 'fst/daq_fst.cc' || echo './'`fst/daq_fst.cc
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO -g -O2 -MT fst/daq_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/daq_fst_la-daq_fst.Tpo -c fst/daq_fst.cc  -fPIC -DPIC -o fst/.libs/daq_fst_la-daq_fst.o
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO -g -O2 -MT fst/daq_fst_la-daq_fst.lo -MD -MP -MF fst/.deps/daq_fst_la-daq_fst.Tpo -c fst/daq_fst.cc -o fst/daq_fst_la-daq_fst.o >/dev/null 2>&1
mv -f fst/.deps/daq_fst_la-daq_fst.Tpo fst/.deps/daq_fst_la-daq_fst.Plo
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/daq_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/daq_fst_la-PMurHash.Tpo -c -o fst/daq_fst_la-PMurHash.lo `test -f 'fst/PMurHash.c' || echo './'`fst/PMurHash.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/daq_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/daq_fst_la-PMurHash.Tpo -c fst/PMurHash.c  -fPIC -DPIC -o fst/.libs/daq_fst_la-PMurHash.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -I../example -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT fst/daq_fst_la-PMurHash.lo -MD -MP -MF fst/.deps/daq_fst_la-PMurHash.Tpo -c fst/PMurHash.c -o fst/daq_fst_la-PMurHash.o >/dev/null 2>&1
mv -f fst/.deps/daq_fst_la-PMurHash.Tpo fst/.deps/daq_fst_la-PMurHash.Plo
/bin/bash ../libtool  --tag=CXX   --mode=link g++ -std=gnu++11  -g -O2 -module -export-dynamic -avoid-version -shared  -o fst/daq_fst.la -rpath /usr/local/lib/daq fst/daq_fst_la-daq_fst.lo fst/daq_fst_la-PMurHash.lo  
libtool: link: g++ -std=gnu++11  -fPIC -DPIC -shared -nostdlib /usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/15/crtbeginS.o  fst/.libs/daq_fst_la-daq_fst.o fst/.libs/daq_fst_la-PMurHash.o   -L/usr/lib/gcc/x86_64-linux-gnu/15 -L/usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/15/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/15/../../.. -L/lib -L/usr/lib -lstdc++ -lm -lc -lgcc_s /usr/lib/gcc/x86_64-linux-gnu/15/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu/crtn.o  -g -O2   -Wl,-soname -Wl,daq_fst.so -o fst/.libs/daq_fst.so
libtool: link: ( cd "fst/.libs" && rm -f "daq_fst.la" && ln -s "../daq_fst.la" "daq_fst.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO   -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/daq_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/daq_pcap_la-daq_pcap.Tpo -c -o pcap/daq_pcap_la-daq_pcap.lo `test -f 'pcap/daq_pcap.c' || echo './'`pcap/daq_pcap.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/daq_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/daq_pcap_la-daq_pcap.Tpo -c pcap/daq_pcap.c  -fPIC -DPIC -o pcap/.libs/daq_pcap_la-daq_pcap.o
pcap/daq_pcap.c: In function 'create_packet_pool':
pcap/daq_pcap.c:126:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  126 |     pool->pool = calloc(sizeof(PcapPktDesc), size);
      |                                ^~~~~~~~~~~
pcap/daq_pcap.c:126:32: note: earlier argument should specify number of elements, later size of each element
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT pcap/daq_pcap_la-daq_pcap.lo -MD -MP -MF pcap/.deps/daq_pcap_la-daq_pcap.Tpo -c pcap/daq_pcap.c -o pcap/daq_pcap_la-daq_pcap.o >/dev/null 2>&1
mv -f pcap/.deps/daq_pcap_la-daq_pcap.Tpo pcap/.deps/daq_pcap_la-daq_pcap.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared   -o pcap/daq_pcap.la -rpath /usr/local/lib/daq pcap/daq_pcap_la-daq_pcap.lo -lpcap -lpthread 
libtool: link: gcc -shared  -fPIC -DPIC  pcap/.libs/daq_pcap_la-daq_pcap.o   -lpcap -lpthread  -g -O2   -Wl,-soname -Wl,daq_pcap.so -o pcap/.libs/daq_pcap.so
libtool: link: ( cd "pcap/.libs" && rm -f "daq_pcap.la" && ln -s "../daq_pcap.la" "daq_pcap.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/daq_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/daq_savefile_la-daq_savefile.Tpo -c -o savefile/daq_savefile_la-daq_savefile.lo `test -f 'savefile/daq_savefile.c' || echo './'`savefile/daq_savefile.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/daq_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/daq_savefile_la-daq_savefile.Tpo -c savefile/daq_savefile.c  -fPIC -DPIC -o savefile/.libs/daq_savefile_la-daq_savefile.o
savefile/daq_savefile.c: In function 'create_message_pool':
savefile/daq_savefile.c:125:32: warning: 'calloc' sizes specified with 'sizeof' in the earlier argument and not in the later argument [-Wcalloc-transposed-args]
  125 |     pool->pool = calloc(sizeof(SavefileMsgDesc), size);
      |                                ^~~~~~~~~~~~~~~
savefile/daq_savefile.c:125:32: note: earlier argument should specify number of elements, later size of each element
savefile/daq_savefile.c: In function 'savefile_read_message':
savefile/daq_savefile.c:167:43: warning: comparison of integer expressions of different signedness: 'long unsigned int' and 'off_t' {aka 'long int'} [-Wsign-compare]
  167 |     if (sfc->file_offset + sizeof(*sfhdr) > sfc->file_size)
      |                                           ^
savefile/daq_savefile.c: In function 'savefile_daq_start':
savefile/daq_savefile.c:315:24: warning: comparison of integer expressions of different signedness: 'off_t' {aka 'long int'} and 'long unsigned int' [-Wsign-compare]
  315 |     if (sfc->file_size < sizeof(struct pcap_file_header))
      |                        ^
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT savefile/daq_savefile_la-daq_savefile.lo -MD -MP -MF savefile/.deps/daq_savefile_la-daq_savefile.Tpo -c savefile/daq_savefile.c -o savefile/daq_savefile_la-daq_savefile.o >/dev/null 2>&1
mv -f savefile/.deps/daq_savefile_la-daq_savefile.Tpo savefile/.deps/daq_savefile_la-daq_savefile.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared  -o savefile/daq_savefile.la -rpath /usr/local/lib/daq savefile/daq_savefile_la-daq_savefile.lo  
libtool: link: gcc -shared  -fPIC -DPIC  savefile/.libs/daq_savefile_la-daq_savefile.o    -g -O2   -Wl,-soname -Wl,daq_savefile.so -o savefile/.libs/daq_savefile.so
libtool: link: ( cd "savefile/.libs" && rm -f "daq_savefile.la" && ln -s "../daq_savefile.la" "daq_savefile.la" )
/bin/bash ../libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO  -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/daq_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/daq_trace_la-daq_trace.Tpo -c -o trace/daq_trace_la-daq_trace.lo `test -f 'trace/daq_trace.c' || echo './'`trace/daq_trace.c
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/daq_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/daq_trace_la-daq_trace.Tpo -c trace/daq_trace.c  -fPIC -DPIC -o trace/.libs/daq_trace_la-daq_trace.o
libtool: compile:  gcc -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -MT trace/daq_trace_la-daq_trace.lo -MD -MP -MF trace/.deps/daq_trace_la-daq_trace.Tpo -c trace/daq_trace.c -o trace/daq_trace_la-daq_trace.o >/dev/null 2>&1
mv -f trace/.deps/daq_trace_la-daq_trace.Tpo trace/.deps/daq_trace_la-daq_trace.Plo
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wstrict-prototypes -Wmissing-prototypes -Wold-style-definition -Wnested-externs -g -O2 -module -export-dynamic -avoid-version -shared  -o trace/daq_trace.la -rpath /usr/local/lib/daq trace/daq_trace_la-daq_trace.lo  
libtool: link: gcc -shared  -fPIC -DPIC  trace/.libs/daq_trace_la-daq_trace.o    -g -O2   -Wl,-soname -Wl,daq_trace.so -o trace/.libs/daq_trace.so
libtool: link: ( cd "trace/.libs" && rm -f "daq_trace.la" && ln -s "../daq_trace.la" "daq_trace.la" )
/bin/bash ../libtool  --tag=CXX   --mode=compile g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO   -g -O2 -MT gwlb/daq_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/daq_gwlb_la-daq_gwlb.Tpo -c -o gwlb/daq_gwlb_la-daq_gwlb.lo `test -f 'gwlb/daq_gwlb.cc' || echo './'`gwlb/daq_gwlb.cc
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -g -O2 -MT gwlb/daq_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/daq_gwlb_la-daq_gwlb.Tpo -c gwlb/daq_gwlb.cc  -fPIC -DPIC -o gwlb/.libs/daq_gwlb_la-daq_gwlb.o
libtool: compile:  g++ -std=gnu++11 -DHAVE_CONFIG_H -I. -I.. -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option -I../api -DBUILDING_SO -g -O2 -MT gwlb/daq_gwlb_la-daq_gwlb.lo -MD -MP -MF gwlb/.deps/daq_gwlb_la-daq_gwlb.Tpo -c gwlb/daq_gwlb.cc -o gwlb/daq_gwlb_la-daq_gwlb.o >/dev/null 2>&1
mv -f gwlb/.deps/daq_gwlb_la-daq_gwlb.Tpo gwlb/.deps/daq_gwlb_la-daq_gwlb.Plo
/bin/bash ../libtool  --tag=CXX   --mode=link g++ -std=gnu++11  -g -O2 -module -export-dynamic -avoid-version -shared  -o gwlb/daq_gwlb.la -rpath /usr/local/lib/daq gwlb/daq_gwlb_la-daq_gwlb.lo  
libtool: link: g++ -std=gnu++11  -fPIC -DPIC -shared -nostdlib /usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/15/crtbeginS.o  gwlb/.libs/daq_gwlb_la-daq_gwlb.o   -L/usr/lib/gcc/x86_64-linux-gnu/15 -L/usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/15/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/15/../../.. -L/lib -L/usr/lib -lstdc++ -lm -lc -lgcc_s /usr/lib/gcc/x86_64-linux-gnu/15/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/15/../../../x86_64-linux-gnu/crtn.o  -g -O2   -Wl,-soname -Wl,daq_gwlb.so -o gwlb/.libs/daq_gwlb.so
libtool: link: ( cd "gwlb/.libs" && rm -f "daq_gwlb.la" && ln -s "../daq_gwlb.la" "daq_gwlb.la" )
make[2]: Leaving directory '/home/kali/snort_src/daq/modules'
Making all in example
make[2]: Entering directory '/home/kali/snort_src/daq/example'
gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option  -Wall -I../api -g -O2 -MT daqtest.o -MD -MP -MF .deps/daqtest.Tpo -c -o daqtest.o daqtest.c
daqtest.c: In function ‘replace_icmp_data’:
daqtest.c:309:12: warning: cast discards ‘const’ qualifier from pointer target type [-Wcast-qual]
  309 |     icmp = (IcmpHdr *) dtp->dd.icmp;
      |            ^
mv -f .deps/daqtest.Tpo .deps/daqtest.Po
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wall -I../api -g -O2   -o daqtest daqtest.o ../api/libdaq.la -lpthread 
libtool: link: gcc -Wall -I../api -g -O2 -o .libs/daqtest daqtest.o  ../api/.libs/libdaq.so -lpthread
gcc -DHAVE_CONFIG_H -I. -I..  -fvisibility=hidden -Wall -Wmissing-declarations -Wpointer-arith -Wcast-align -Wcast-qual -Wformat -Wformat-nonliteral -Wformat-security -Wundef -Wwrite-strings -Wextra -Wsign-compare -Wno-unused-parameter -fno-strict-aliasing -fdiagnostics-show-option  -Wall -I../api -DUSE_STATIC_MODULES -DBUILD_AFPACKET_MODULE -DBUILD_BPF_MODULE  -DBUILD_DUMP_MODULE -DBUILD_FST_MODULE   -DBUILD_PCAP_MODULE -DBUILD_SAVEFILE_MODULE -DBUILD_TRACE_MODULE -g -O2 -MT daqtest_static-daqtest.o -MD -MP -MF .deps/daqtest_static-daqtest.Tpo -c -o daqtest_static-daqtest.o `test -f 'daqtest.c' || echo './'`daqtest.c
daqtest.c: In function ‘replace_icmp_data’:
daqtest.c:309:12: warning: cast discards ‘const’ qualifier from pointer target type [-Wcast-qual]
  309 |     icmp = (IcmpHdr *) dtp->dd.icmp;
      |            ^
mv -f .deps/daqtest_static-daqtest.Tpo .deps/daqtest_static-daqtest.Po
/bin/bash ../libtool  --tag=CC   --mode=link gcc -Wall -I../api -DUSE_STATIC_MODULES -DBUILD_AFPACKET_MODULE -DBUILD_BPF_MODULE  -DBUILD_DUMP_MODULE -DBUILD_FST_MODULE   -DBUILD_PCAP_MODULE -DBUILD_SAVEFILE_MODULE -DBUILD_TRACE_MODULE -g -O2 -static-libtool-libs   -o daqtest-static daqtest_static-daqtest.o ../api/libdaq.la -lpthread ../modules/afpacket/libdaq_static_afpacket.la -lpcap -lpthread ../modules/bpf/libdaq_static_bpf.la -lpcap -lpthread  ../modules/dump/libdaq_static_dump.la -lpcap ../modules/fst/libdaq_static_fst.la -lstdc++   ../modules/pcap/libdaq_static_pcap.la -lpcap -lpthread ../modules/savefile/libdaq_static_savefile.la ../modules/trace/libdaq_static_trace.la 
libtool: link: gcc -Wall -I../api -DUSE_STATIC_MODULES -DBUILD_AFPACKET_MODULE -DBUILD_BPF_MODULE -DBUILD_DUMP_MODULE -DBUILD_FST_MODULE -DBUILD_PCAP_MODULE -DBUILD_SAVEFILE_MODULE -DBUILD_TRACE_MODULE -g -O2 -o daqtest-static daqtest_static-daqtest.o  ../api/.libs/libdaq.a -ldl ../modules/afpacket/.libs/libdaq_static_afpacket.a ../modules/bpf/.libs/libdaq_static_bpf.a ../modules/dump/.libs/libdaq_static_dump.a ../modules/fst/.libs/libdaq_static_fst.a -lstdc++ ../modules/pcap/.libs/libdaq_static_pcap.a -lpcap -lpthread ../modules/savefile/.libs/libdaq_static_savefile.a ../modules/trace/.libs/libdaq_static_trace.a
make[2]: Leaving directory '/home/kali/snort_src/daq/example'
Making all in test
make[2]: Entering directory '/home/kali/snort_src/daq/test'
make[2]: Nothing to be done for 'all'.
make[2]: Leaving directory '/home/kali/snort_src/daq/test'
make[2]: Entering directory '/home/kali/snort_src/daq'
make[2]: Leaving directory '/home/kali/snort_src/daq'
make[1]: Leaving directory '/home/kali/snort_src/daq'
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ sudo make install
[sudo] password for kali: 
Making install in api
make[1]: Entering directory '/home/kali/snort_src/daq/api'
make[2]: Entering directory '/home/kali/snort_src/daq/api'
 /usr/bin/mkdir -p '/usr/local/lib'
 /bin/bash ../libtool   --mode=install /usr/bin/install -c   libdaq.la '/usr/local/lib'
libtool: install: /usr/bin/install -c .libs/libdaq.so.3.0.0 /usr/local/lib/libdaq.so.3.0.0
libtool: install: (cd /usr/local/lib && { ln -s -f libdaq.so.3.0.0 libdaq.so.3 || { rm -f libdaq.so.3 && ln -s libdaq.so.3.0.0 libdaq.so.3; }; })
libtool: install: (cd /usr/local/lib && { ln -s -f libdaq.so.3.0.0 libdaq.so || { rm -f libdaq.so && ln -s libdaq.so.3.0.0 libdaq.so; }; })
libtool: install: /usr/bin/install -c .libs/libdaq.lai /usr/local/lib/libdaq.la
libtool: install: /usr/bin/install -c .libs/libdaq.a /usr/local/lib/libdaq.a
libtool: install: chmod 644 /usr/local/lib/libdaq.a
libtool: install: ranlib /usr/local/lib/libdaq.a
libtool: finish: PATH="/usr/sbin:/usr/bin:/sbin:/bin:/sbin" ldconfig -n /usr/local/lib
----------------------------------------------------------------------
Libraries have been installed in:
   /usr/local/lib

If you ever happen to want to link against installed libraries
in a given directory, LIBDIR, you must either use libtool, and
specify the full pathname of the library, or use the '-LLIBDIR'
flag during linking and do at least one of the following:
   - add LIBDIR to the 'LD_LIBRARY_PATH' environment variable
     during execution
   - add LIBDIR to the 'LD_RUN_PATH' environment variable
     during linking
   - use the '-Wl,-rpath -Wl,LIBDIR' linker flag
   - have your system administrator add LIBDIR to '/etc/ld.so.conf'

See any operating system documentation about shared libraries for
more information, such as the ld(1) and ld.so(8) manual pages.
----------------------------------------------------------------------
 /usr/bin/mkdir -p '/usr/local/include'
 /usr/bin/install -c -m 644 daq.h daq_common.h daq_dlt.h daq_module_api.h daq_version.h '/usr/local/include'
make[2]: Leaving directory '/home/kali/snort_src/daq/api'
make[1]: Leaving directory '/home/kali/snort_src/daq/api'
Making install in modules
make[1]: Entering directory '/home/kali/snort_src/daq/modules'
make[2]: Entering directory '/home/kali/snort_src/daq/modules'
 /usr/bin/mkdir -p '/usr/local/lib'
 /bin/bash ../libtool   --mode=install /usr/bin/install -c   afpacket/libdaq_static_afpacket.la bpf/libdaq_static_bpf.la dump/libdaq_static_dump.la fst/libdaq_static_fst.la pcap/libdaq_static_pcap.la savefile/libdaq_static_savefile.la trace/libdaq_static_trace.la gwlb/libdaq_static_gwlb.la '/usr/local/lib'
libtool: install: /usr/bin/install -c afpacket/.libs/libdaq_static_afpacket.lai /usr/local/lib/libdaq_static_afpacket.la
libtool: install: /usr/bin/install -c bpf/.libs/libdaq_static_bpf.lai /usr/local/lib/libdaq_static_bpf.la
libtool: install: /usr/bin/install -c dump/.libs/libdaq_static_dump.lai /usr/local/lib/libdaq_static_dump.la
libtool: install: /usr/bin/install -c fst/.libs/libdaq_static_fst.lai /usr/local/lib/libdaq_static_fst.la
libtool: install: /usr/bin/install -c pcap/.libs/libdaq_static_pcap.lai /usr/local/lib/libdaq_static_pcap.la
libtool: install: /usr/bin/install -c savefile/.libs/libdaq_static_savefile.lai /usr/local/lib/libdaq_static_savefile.la
libtool: install: /usr/bin/install -c trace/.libs/libdaq_static_trace.lai /usr/local/lib/libdaq_static_trace.la
libtool: install: /usr/bin/install -c gwlb/.libs/libdaq_static_gwlb.lai /usr/local/lib/libdaq_static_gwlb.la
libtool: install: /usr/bin/install -c afpacket/.libs/libdaq_static_afpacket.a /usr/local/lib/libdaq_static_afpacket.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_afpacket.a
libtool: install: ranlib /usr/local/lib/libdaq_static_afpacket.a
libtool: install: /usr/bin/install -c bpf/.libs/libdaq_static_bpf.a /usr/local/lib/libdaq_static_bpf.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_bpf.a
libtool: install: ranlib /usr/local/lib/libdaq_static_bpf.a
libtool: install: /usr/bin/install -c dump/.libs/libdaq_static_dump.a /usr/local/lib/libdaq_static_dump.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_dump.a
libtool: install: ranlib /usr/local/lib/libdaq_static_dump.a
libtool: install: /usr/bin/install -c fst/.libs/libdaq_static_fst.a /usr/local/lib/libdaq_static_fst.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_fst.a
libtool: install: ranlib /usr/local/lib/libdaq_static_fst.a
libtool: install: /usr/bin/install -c pcap/.libs/libdaq_static_pcap.a /usr/local/lib/libdaq_static_pcap.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_pcap.a
libtool: install: ranlib /usr/local/lib/libdaq_static_pcap.a
libtool: install: /usr/bin/install -c savefile/.libs/libdaq_static_savefile.a /usr/local/lib/libdaq_static_savefile.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_savefile.a
libtool: install: ranlib /usr/local/lib/libdaq_static_savefile.a
libtool: install: /usr/bin/install -c trace/.libs/libdaq_static_trace.a /usr/local/lib/libdaq_static_trace.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_trace.a
libtool: install: ranlib /usr/local/lib/libdaq_static_trace.a
libtool: install: /usr/bin/install -c gwlb/.libs/libdaq_static_gwlb.a /usr/local/lib/libdaq_static_gwlb.a
libtool: install: chmod 644 /usr/local/lib/libdaq_static_gwlb.a
libtool: install: ranlib /usr/local/lib/libdaq_static_gwlb.a
libtool: finish: PATH="/usr/sbin:/usr/bin:/sbin:/bin:/sbin" ldconfig -n /usr/local/lib
----------------------------------------------------------------------
Libraries have been installed in:
   /usr/local/lib

If you ever happen to want to link against installed libraries
in a given directory, LIBDIR, you must either use libtool, and
specify the full pathname of the library, or use the '-LLIBDIR'
flag during linking and do at least one of the following:
   - add LIBDIR to the 'LD_LIBRARY_PATH' environment variable
     during execution
   - add LIBDIR to the 'LD_RUN_PATH' environment variable
     during linking
   - use the '-Wl,-rpath -Wl,LIBDIR' linker flag
   - have your system administrator add LIBDIR to '/etc/ld.so.conf'

See any operating system documentation about shared libraries for
more information, such as the ld(1) and ld.so(8) manual pages.
----------------------------------------------------------------------
 /usr/bin/mkdir -p '/usr/local/lib/daq'
 /bin/bash ../libtool   --mode=install /usr/bin/install -c   afpacket/daq_afpacket.la bpf/daq_bpf.la dump/daq_dump.la fst/daq_fst.la pcap/daq_pcap.la savefile/daq_savefile.la trace/daq_trace.la gwlb/daq_gwlb.la '/usr/local/lib/daq'
libtool: install: /usr/bin/install -c afpacket/.libs/daq_afpacket.so /usr/local/lib/daq/daq_afpacket.so
libtool: install: /usr/bin/install -c afpacket/.libs/daq_afpacket.lai /usr/local/lib/daq/daq_afpacket.la
libtool: install: /usr/bin/install -c bpf/.libs/daq_bpf.so /usr/local/lib/daq/daq_bpf.so
libtool: install: /usr/bin/install -c bpf/.libs/daq_bpf.lai /usr/local/lib/daq/daq_bpf.la
libtool: install: /usr/bin/install -c dump/.libs/daq_dump.so /usr/local/lib/daq/daq_dump.so
libtool: install: /usr/bin/install -c dump/.libs/daq_dump.lai /usr/local/lib/daq/daq_dump.la
libtool: install: /usr/bin/install -c fst/.libs/daq_fst.so /usr/local/lib/daq/daq_fst.so
libtool: install: /usr/bin/install -c fst/.libs/daq_fst.lai /usr/local/lib/daq/daq_fst.la
libtool: install: /usr/bin/install -c pcap/.libs/daq_pcap.so /usr/local/lib/daq/daq_pcap.so
libtool: install: /usr/bin/install -c pcap/.libs/daq_pcap.lai /usr/local/lib/daq/daq_pcap.la
libtool: install: /usr/bin/install -c savefile/.libs/daq_savefile.so /usr/local/lib/daq/daq_savefile.so
libtool: install: /usr/bin/install -c savefile/.libs/daq_savefile.lai /usr/local/lib/daq/daq_savefile.la
libtool: install: /usr/bin/install -c trace/.libs/daq_trace.so /usr/local/lib/daq/daq_trace.so
libtool: install: /usr/bin/install -c trace/.libs/daq_trace.lai /usr/local/lib/daq/daq_trace.la
libtool: install: /usr/bin/install -c gwlb/.libs/daq_gwlb.so /usr/local/lib/daq/daq_gwlb.so
libtool: install: /usr/bin/install -c gwlb/.libs/daq_gwlb.lai /usr/local/lib/daq/daq_gwlb.la
libtool: finish: PATH="/usr/sbin:/usr/bin:/sbin:/bin:/sbin" ldconfig -n /usr/local/lib/daq
----------------------------------------------------------------------
Libraries have been installed in:
   /usr/local/lib/daq

If you ever happen to want to link against installed libraries
in a given directory, LIBDIR, you must either use libtool, and
specify the full pathname of the library, or use the '-LLIBDIR'
flag during linking and do at least one of the following:
   - add LIBDIR to the 'LD_LIBRARY_PATH' environment variable
     during execution
   - add LIBDIR to the 'LD_RUN_PATH' environment variable
     during linking
   - use the '-Wl,-rpath -Wl,LIBDIR' linker flag
   - have your system administrator add LIBDIR to '/etc/ld.so.conf'

See any operating system documentation about shared libraries for
more information, such as the ld(1) and ld.so(8) manual pages.
----------------------------------------------------------------------
 /usr/bin/mkdir -p '/usr/local/lib/pkgconfig'
 /usr/bin/install -c -m 644 afpacket/libdaq_static_afpacket.pc bpf/libdaq_static_bpf.pc dump/libdaq_static_dump.pc fst/libdaq_static_fst.pc pcap/libdaq_static_pcap.pc savefile/libdaq_static_savefile.pc trace/libdaq_static_trace.pc gwlb/libdaq_static_gwlb.pc '/usr/local/lib/pkgconfig'
make[2]: Leaving directory '/home/kali/snort_src/daq/modules'
make[1]: Leaving directory '/home/kali/snort_src/daq/modules'
Making install in example
make[1]: Entering directory '/home/kali/snort_src/daq/example'
make[2]: Entering directory '/home/kali/snort_src/daq/example'
 /usr/bin/mkdir -p '/usr/local/bin'
  /bin/bash ../libtool   --mode=install /usr/bin/install -c daqtest daqtest-static '/usr/local/bin'
libtool: install: /usr/bin/install -c .libs/daqtest /usr/local/bin/daqtest
libtool: install: /usr/bin/install -c daqtest-static /usr/local/bin/daqtest-static
make[2]: Nothing to be done for 'install-data-am'.
make[2]: Leaving directory '/home/kali/snort_src/daq/example'
make[1]: Leaving directory '/home/kali/snort_src/daq/example'
Making install in test
make[1]: Entering directory '/home/kali/snort_src/daq/test'
make[2]: Entering directory '/home/kali/snort_src/daq/test'
make[2]: Nothing to be done for 'install-exec-am'.
make[2]: Nothing to be done for 'install-data-am'.
make[2]: Leaving directory '/home/kali/snort_src/daq/test'
make[1]: Leaving directory '/home/kali/snort_src/daq/test'
make[1]: Entering directory '/home/kali/snort_src/daq'
make[2]: Entering directory '/home/kali/snort_src/daq'
make[2]: Nothing to be done for 'install-exec-am'.
 /usr/bin/mkdir -p '/usr/local/lib/pkgconfig'
 /usr/bin/install -c -m 644 libdaq.pc '/usr/local/lib/pkgconfig'
make[2]: Leaving directory '/home/kali/snort_src/daq'
make[1]: Leaving directory '/home/kali/snort_src/daq'
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ sudo ldconfig
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ daq-modules-config --version
                                                                           
┌──(kali㉿kali)-[~/snort_src/daq]
└─$ pkg-config --modversion libdaq
3.0.27







┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo make install
[sudo] password for kali: 
[  0%] Built target unixdomain_connector
[  2%] Built target framework
[  2%] Built target mp_unix_transport
[  3%] Built target ips_actions
[  3%] Built target codecs
[  3%] Built target root_codecs
[  4%] Built target link_codecs
[  6%] Built target ip_codecs
[  7%] Built target misc_codecs
[  7%] Built target control
[ 10%] Built target detection
[ 10%] Built target dump_config
[ 11%] Built target events
[ 13%] Built target file_api
[ 13%] Built target filter
[ 14%] Built target flow
[ 15%] Built target hash
[ 16%] Built target js_norm
[ 16%] Built target latency
[ 17%] Built target log
[ 19%] Built target main
[ 20%] Built target managers
[ 21%] Built target memory
[ 22%] Built target mime
[ 23%] Built target packet_io
[ 24%] Built target parser
[ 25%] Built target payload_injector
[ 26%] Built target ports
[ 27%] Built target protocols
[ 27%] Built target sfip
[ 27%] Built target sfrt
[ 27%] Built target service_inspectors
[ 27%] Built target back_orifice
[ 29%] Built target cip
[ 32%] Built target dce_rpc
[ 32%] Built target dnp3
[ 34%] Built target dns
[ 35%] Built target ftp_telnet
[ 36%] Built target gtp_inspect
[ 40%] Built target http_inspect
[ 42%] Built target http2_inspect
[ 43%] Built target iec104
[ 43%] Built target imap
[ 44%] Built target mms
[ 44%] Built target modbus
[ 44%] Built target netflow
[ 45%] Built target opcua
[ 45%] Built target pop
[ 45%] Built target rpc_decode
[ 46%] Built target s7commplus
[ 47%] Built target sip
[ 47%] Built target smtp
[ 47%] Built target ssh
[ 48%] Built target ssl
[ 48%] Built target tlv_pdu
[ 50%] Built target wizard
[ 51%] Built target socks
[ 51%] Built target stream
[ 52%] Built target stream_paf
[ 52%] Built target stream_base
[ 52%] Built target stream_ip
[ 52%] Built target stream_icmp
[ 55%] Built target stream_tcp
[ 56%] Built target stream_udp
[ 56%] Built target stream_user
[ 57%] Built target stream_file
[ 57%] Built target target_based
[ 58%] Built target host_tracker
[ 59%] Built target pub_sub
[ 60%] Built target time
[ 61%] Built target profiler
[ 61%] Built target trace
[ 62%] Built target tracer
[ 62%] Built target utils
[ 63%] Built target helpers
[ 63%] Built target lua
[ 63%] Built target decompress
[ 69%] Built target ips_options
[ 70%] Built target loggers
[ 70%] Built target network_inspectors
[ 78%] Built target appid
[ 78%] Built target arp_spoof
[ 78%] Built target binder
[ 79%] Built target extractor
[ 79%] Built target normalize
[ 79%] Built target packet_capture
[ 80%] Built target perf_monitor
[ 80%] Built target port_scan
[ 80%] Built target reputation
[ 82%] Built target rna
[ 82%] Built target policy_selectors
[ 82%] Built target address_space_selector
[ 82%] Built target tenant_selector
[ 83%] Built target search_engines
[ 84%] Built target side_channel
[ 84%] Built target connectors
[ 84%] Built target file_connector
[ 84%] Built target tcp_connector
[ 84%] Built target std_connector
[ 85%] Built target mp_transports
[ 85%] Built target snort
[ 85%] Built target api_options
[ 85%] Built target snort_api
[ 85%] Built target u2boat
[ 85%] Built target u2spewfoo
[ 87%] Built target rule_states
[ 90%] Built target config_states
[ 91%] Built target conversion_data
[ 92%] Built target data_types
[ 92%] Built target snort2lua_helpers
[ 94%] Built target keyword_states
[ 95%] Built target output_states
[ 98%] Built target preprocessor_states
[100%] Built target snort2lua
[100%] Built target show_flows
[100%] Built target daq_file
[100%] Built target daq_hext
Install the project...
-- Install configuration: ""
-- Up-to-date: /usr/local/lib/pkgconfig/snort.pc
-- Up-to-date: /usr/local/bin/snort
-- Up-to-date: /usr/local/include/snort/codecs/codec_module.h
-- Up-to-date: /usr/local/include/snort/control/control.h
-- Up-to-date: /usr/local/include/snort/detection/detection_buf.h
-- Up-to-date: /usr/local/include/snort/detection/detection_engine.h
-- Up-to-date: /usr/local/include/snort/detection/extract.h
-- Up-to-date: /usr/local/include/snort/detection/ips_context.h
-- Up-to-date: /usr/local/include/snort/detection/ips_context_chain.h
-- Up-to-date: /usr/local/include/snort/detection/ips_context_data.h
-- Up-to-date: /usr/local/include/snort/detection/pattern_match_data.h
-- Up-to-date: /usr/local/include/snort/detection/rule_option_types.h
-- Up-to-date: /usr/local/include/snort/events/event.h
-- Up-to-date: /usr/local/include/snort/file_api/file_api.h
-- Up-to-date: /usr/local/include/snort/file_api/file_capture.h
-- Up-to-date: /usr/local/include/snort/file_api/file_flows.h
-- Up-to-date: /usr/local/include/snort/file_api/file_lib.h
-- Up-to-date: /usr/local/include/snort/file_api/file_service.h
-- Up-to-date: /usr/local/include/snort/flow/deferred_trust.h
-- Up-to-date: /usr/local/include/snort/flow/dump_flows.h
-- Up-to-date: /usr/local/include/snort/flow/dump_flows_descriptor.h
-- Up-to-date: /usr/local/include/snort/flow/dump_flows_serializer.h
-- Up-to-date: /usr/local/include/snort/flow/expect_flow.h
-- Up-to-date: /usr/local/include/snort/flow/flow.h
-- Up-to-date: /usr/local/include/snort/flow/flow_data.h
-- Up-to-date: /usr/local/include/snort/flow/flow_key.h
-- Up-to-date: /usr/local/include/snort/flow/flow_stash.h
-- Up-to-date: /usr/local/include/snort/flow/ha.h
-- Up-to-date: /usr/local/include/snort/flow/prune_stats.h
-- Up-to-date: /usr/local/include/snort/flow/session.h
-- Up-to-date: /usr/local/include/snort/flow/stream_flow.h
-- Up-to-date: /usr/local/include/snort/framework/base_api.h
-- Up-to-date: /usr/local/include/snort/framework/codec.h
-- Up-to-date: /usr/local/include/snort/framework/connector.h
-- Up-to-date: /usr/local/include/snort/framework/counts.h
-- Up-to-date: /usr/local/include/snort/framework/cursor.h
-- Up-to-date: /usr/local/include/snort/framework/data_bus.h
-- Up-to-date: /usr/local/include/snort/framework/decode_data.h
-- Up-to-date: /usr/local/include/snort/framework/endianness.h
-- Up-to-date: /usr/local/include/snort/framework/inspector.h
-- Up-to-date: /usr/local/include/snort/framework/ips_action.h
-- Up-to-date: /usr/local/include/snort/framework/ips_option.h
-- Up-to-date: /usr/local/include/snort/framework/logger.h
-- Up-to-date: /usr/local/include/snort/framework/module.h
-- Up-to-date: /usr/local/include/snort/framework/mp_data_bus.h
-- Up-to-date: /usr/local/include/snort/framework/mp_transport.h
-- Up-to-date: /usr/local/include/snort/framework/mpse_batch.h
-- Up-to-date: /usr/local/include/snort/framework/mpse.h
-- Up-to-date: /usr/local/include/snort/framework/parameter.h
-- Up-to-date: /usr/local/include/snort/framework/pdu_section.h
-- Up-to-date: /usr/local/include/snort/framework/pig_pen.h
-- Up-to-date: /usr/local/include/snort/framework/plugins.h
-- Up-to-date: /usr/local/include/snort/framework/policy_selector.h
-- Up-to-date: /usr/local/include/snort/framework/range.h
-- Up-to-date: /usr/local/include/snort/framework/so_rule.h
-- Up-to-date: /usr/local/include/snort/framework/tracer.h
-- Up-to-date: /usr/local/include/snort/framework/value.h
-- Up-to-date: /usr/local/include/snort/framework/api_options.h
-- Up-to-date: /usr/local/include/snort/framework/snort_api.h
-- Up-to-date: /usr/local/include/snort/hash/hashes.h
-- Up-to-date: /usr/local/include/snort/hash/hash_key_operations.h
-- Up-to-date: /usr/local/include/snort/hash/lru_cache_local.h
-- Up-to-date: /usr/local/include/snort/hash/lru_cache_shared.h
-- Up-to-date: /usr/local/include/snort/hash/lru_segmented_cache_shared.h
-- Up-to-date: /usr/local/include/snort/hash/xhash.h
-- Up-to-date: /usr/local/include/snort/log/log_stats.h
-- Up-to-date: /usr/local/include/snort/log/log_text.h
-- Up-to-date: /usr/local/include/snort/log/messages.h
-- Up-to-date: /usr/local/include/snort/log/obfuscator.h
-- Up-to-date: /usr/local/include/snort/log/text_log.h
-- Up-to-date: /usr/local/include/snort/log/unified2.h
-- Up-to-date: /usr/local/include/snort/log/u2_packet.h
-- Up-to-date: /usr/local/include/snort/main/analyzer_command.h
-- Up-to-date: /usr/local/include/snort/main/policy.h
-- Up-to-date: /usr/local/include/snort/main/reload_tracker.h
-- Up-to-date: /usr/local/include/snort/main/reload_tuner.h
-- Up-to-date: /usr/local/include/snort/main/snort_config.h
-- Up-to-date: /usr/local/include/snort/main/snort_types.h
-- Up-to-date: /usr/local/include/snort/main/thread.h
-- Up-to-date: /usr/local/include/snort/main/thread_config.h
-- Up-to-date: /usr/local/include/snort/main/snort.h
-- Up-to-date: /usr/local/include/snort/lua/snort_plugin.lua
-- Up-to-date: /usr/local/include/snort/memory/heap_interface.h
-- Up-to-date: /usr/local/include/snort/memory/memory_cap.h
-- Up-to-date: /usr/local/include/snort/mime/decode_b64.h
-- Up-to-date: /usr/local/include/snort/mime/decode_base.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_config.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_decode.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_form_data.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_log.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_paf.h
-- Up-to-date: /usr/local/include/snort/mime/file_mime_process.h
-- Up-to-date: /usr/local/include/snort/packet_io/active.h
-- Up-to-date: /usr/local/include/snort/packet_io/active_action.h
-- Up-to-date: /usr/local/include/snort/packet_io/packet_constraints.h
-- Up-to-date: /usr/local/include/snort/packet_io/packet_tracer.h
-- Up-to-date: /usr/local/include/snort/packet_io/sfdaq.h
-- Up-to-date: /usr/local/include/snort/packet_io/sfdaq_instance.h
-- Up-to-date: /usr/local/include/snort/payload_injector/payload_injector.h
-- Up-to-date: /usr/local/include/snort/protocols/arp.h
-- Up-to-date: /usr/local/include/snort/protocols/bpdu.h
-- Up-to-date: /usr/local/include/snort/protocols/cdp.h
-- Up-to-date: /usr/local/include/snort/protocols/cisco_meta_data.h
-- Up-to-date: /usr/local/include/snort/protocols/eapol.h
-- Up-to-date: /usr/local/include/snort/protocols/eth.h
-- Up-to-date: /usr/local/include/snort/protocols/icmp4.h
-- Up-to-date: /usr/local/include/snort/protocols/icmp6.h
-- Up-to-date: /usr/local/include/snort/protocols/ip.h
-- Up-to-date: /usr/local/include/snort/protocols/ipv4.h
-- Up-to-date: /usr/local/include/snort/protocols/ipv4_options.h
-- Up-to-date: /usr/local/include/snort/protocols/ipv6.h
-- Up-to-date: /usr/local/include/snort/protocols/geneve.h
-- Up-to-date: /usr/local/include/snort/protocols/gre.h
-- Up-to-date: /usr/local/include/snort/protocols/layer.h
-- Up-to-date: /usr/local/include/snort/protocols/linux_sll.h
-- Up-to-date: /usr/local/include/snort/protocols/mpls.h
-- Up-to-date: /usr/local/include/snort/protocols/packet.h
-- Up-to-date: /usr/local/include/snort/protocols/packet_manager.h
-- Up-to-date: /usr/local/include/snort/protocols/protocol_ids.h
-- Up-to-date: /usr/local/include/snort/protocols/ssl.h
-- Up-to-date: /usr/local/include/snort/protocols/tcp.h
-- Up-to-date: /usr/local/include/snort/protocols/tcp_options.h
-- Up-to-date: /usr/local/include/snort/protocols/teredo.h
-- Up-to-date: /usr/local/include/snort/protocols/token_ring.h
-- Up-to-date: /usr/local/include/snort/protocols/udp.h
-- Up-to-date: /usr/local/include/snort/protocols/wlan.h
-- Up-to-date: /usr/local/include/snort/protocols/vlan.h
-- Up-to-date: /usr/local/include/snort/sfip/sf_cidr.h
-- Up-to-date: /usr/local/include/snort/sfip/sf_ip.h
-- Up-to-date: /usr/local/include/snort/sfip/sf_returns.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ftp_telnet/ftp_data.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ftp_telnet/ftpdata_splitter.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ftp_telnet/ftp_module.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ftp_telnet/ftpp_ui_config.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ftp_telnet/kmap.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http_inspect/http_field.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http_inspect/http_common.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http_inspect/http_inspect_base.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http_inspect/http_stream_splitter_base.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http_inspect/http_test_manager.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http2_inspect/http2_huffman_state_machine.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_int_decode.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_int_decode_impl.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_string_decode.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_string_decode_impl.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/netflow/netflow_record.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ssh/ssh_types.h
-- Up-to-date: /usr/local/include/snort/service_inspectors/ssl/ssl_flow_data.h
-- Up-to-date: /usr/local/include/snort/stream/flush_bucket.h
-- Up-to-date: /usr/local/include/snort/stream/paf.h
-- Up-to-date: /usr/local/include/snort/stream/pafng.h
-- Up-to-date: /usr/local/include/snort/stream/stream.h
-- Up-to-date: /usr/local/include/snort/stream/stream_splitter.h
-- Up-to-date: /usr/local/include/snort/stream/udp/udp_session.h
-- Up-to-date: /usr/local/include/snort/target_based/snort_protocols.h
-- Up-to-date: /usr/local/include/snort/host_tracker/cache_allocator.h
-- Up-to-date: /usr/local/include/snort/host_tracker/cache_interface.h
-- Up-to-date: /usr/local/include/snort/host_tracker/host_cache.h
-- Up-to-date: /usr/local/include/snort/host_tracker/host_tracker.h
-- Up-to-date: /usr/local/include/snort/pub_sub/appid_debug_log_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/appid_event_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/appid_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/assistant_gadget_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/cip_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/daq_message_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/data_decrypt_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/dcerpc_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/detection_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/dhcp_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/dns_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/domain_fronting.h
-- Up-to-date: /usr/local/include/snort/pub_sub/eof_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/eve_process_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/expect_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/external_event_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/file_events_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/file_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/finalize_packet_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/ftp_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_body_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_event_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_form_data_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_publish_length_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_request_body_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/http_transaction_end_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/intrinsic_event_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/netflow_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/opportunistic_tls_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/packet_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/quic_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/reputation_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/rna_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/shadowtraffic_aggregator.h
-- Up-to-date: /usr/local/include/snort/pub_sub/sip_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/smb_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/ssh_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/ssl_events.h
-- Up-to-date: /usr/local/include/snort/pub_sub/stream_event_ids.h
-- Up-to-date: /usr/local/include/snort/pub_sub/dns_payload_event.h
-- Up-to-date: /usr/local/include/snort/pub_sub/deviceinfo_events.h
-- Up-to-date: /usr/local/include/snort/time/clock_defs.h
-- Up-to-date: /usr/local/include/snort/time/packet_time.h
-- Up-to-date: /usr/local/include/snort/time/periodic.h
-- Up-to-date: /usr/local/include/snort/time/stopwatch.h
-- Up-to-date: /usr/local/include/snort/profiler/memory_defs.h
-- Up-to-date: /usr/local/include/snort/profiler/memory_profiler_defs.h
-- Up-to-date: /usr/local/include/snort/profiler/profiler.h
-- Up-to-date: /usr/local/include/snort/profiler/profiler_defs.h
-- Up-to-date: /usr/local/include/snort/profiler/rule_profiler_defs.h
-- Up-to-date: /usr/local/include/snort/profiler/time_profiler_defs.h
-- Up-to-date: /usr/local/include/snort/trace/trace.h
-- Up-to-date: /usr/local/include/snort/trace/trace_api.h
-- Up-to-date: /usr/local/include/snort/utils/bits.h
-- Up-to-date: /usr/local/include/snort/utils/cpp_macros.h
-- Up-to-date: /usr/local/include/snort/utils/endian.h
-- Up-to-date: /usr/local/include/snort/utils/safec.h
-- Up-to-date: /usr/local/include/snort/utils/util.h
-- Up-to-date: /usr/local/include/snort/utils/util_cstring.h
-- Up-to-date: /usr/local/include/snort/utils/util_unfold.h
-- Up-to-date: /usr/local/include/snort/helpers/base64_encoder.h
-- Up-to-date: /usr/local/include/snort/helpers/ber.h
-- Up-to-date: /usr/local/include/snort/helpers/bitop.h
-- Up-to-date: /usr/local/include/snort/helpers/boyer_moore.h
-- Up-to-date: /usr/local/include/snort/helpers/boyer_moore_search.h
-- Up-to-date: /usr/local/include/snort/helpers/buffer_data.h
-- Up-to-date: /usr/local/include/snort/helpers/event_gen.h
-- Up-to-date: /usr/local/include/snort/helpers/infractions.h
-- Up-to-date: /usr/local/include/snort/helpers/json_stream.h
-- Up-to-date: /usr/local/include/snort/helpers/literal_search.h
-- Up-to-date: /usr/local/include/snort/helpers/lockless_ring.h
-- Up-to-date: /usr/local/include/snort/helpers/memcap_allocator.h
-- Up-to-date: /usr/local/include/snort/helpers/ring2.h
-- Up-to-date: /usr/local/include/snort/helpers/scratch_allocator.h
-- Up-to-date: /usr/local/include/snort/helpers/sigsafe.h
-- Up-to-date: /usr/local/include/snort/helpers/utf.h
-- Up-to-date: /usr/local/include/snort/decompress/file_decomp.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_api.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_app_descriptor.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_debug.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_dns_session.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_http_session.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_session_api.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/appid_types.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/application_ids.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/tp_appid_module_api.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/tp_appid_session_api.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/tp_appid_types.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/mp_data_bus.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/appid/mp_data_bus.cc
-- Up-to-date: /usr/local/include/snort/network_inspectors/extractor/extractor_enums.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/reputation/reputation_common.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_cpe_os.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_deviceinfo.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_smb.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_tcp.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_ua.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_udp.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_inspector.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_logger_event.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_name.h
-- Up-to-date: /usr/local/include/snort/network_inspectors/rna/rna_tracker.h
-- Up-to-date: /usr/local/include/snort/search_engines/search_common.h
-- Up-to-date: /usr/local/include/snort/search_engines/search_tool.h
-- Up-to-date: /usr/local/bin/appid_detector_builder.sh
-- Up-to-date: /usr/local/bin/u2boat
-- Up-to-date: /usr/local/share/doc/snort/README.u2boat
-- Up-to-date: /usr/local/bin/u2spewfoo
-- Up-to-date: /usr/local/bin/snort2lua
-- Up-to-date: /usr/local/bin/show_flows
-- Up-to-date: /usr/local/share/doc/snort/README.show_flows
-- Up-to-date: /usr/local/etc/snort/balanced.lua
-- Up-to-date: /usr/local/etc/snort/connectivity.lua
-- Up-to-date: /usr/local/etc/snort/file_magic.rules
-- Up-to-date: /usr/local/etc/snort/inline.lua
-- Up-to-date: /usr/local/etc/snort/max_detect.lua
-- Up-to-date: /usr/local/etc/snort/sensitive_data.rules
-- Up-to-date: /usr/local/etc/snort/security.lua
-- Up-to-date: /usr/local/etc/snort/snort.lua
-- Up-to-date: /usr/local/etc/snort/snort_defaults.lua
-- Up-to-date: /usr/local/etc/snort/talos.lua
-- Up-to-date: /usr/local/lib/snort/daq/daq_file.so
-- Up-to-date: /usr/local/lib/snort/daq/daq_hext.so
-- Up-to-date: /usr/local/include/snort/daq/daq_user.h
-- Up-to-date: /usr/local/share/doc/snort/active.txt
-- Up-to-date: /usr/local/share/doc/snort/appid.txt
-- Up-to-date: /usr/local/share/doc/snort/binder.txt
-- Up-to-date: /usr/local/share/doc/snort/byte_extract.txt
-- Up-to-date: /usr/local/share/doc/snort/byte_jump.txt
-- Up-to-date: /usr/local/share/doc/snort/byte_math.txt
-- Up-to-date: /usr/local/share/doc/snort/byte_options.txt
-- Up-to-date: /usr/local/share/doc/snort/byte_test.txt
-- Up-to-date: /usr/local/share/doc/snort/concepts.txt
-- Up-to-date: /usr/local/share/doc/snort/connectors.txt
-- Up-to-date: /usr/local/share/doc/snort/dump_config.txt
-- Up-to-date: /usr/local/share/doc/snort/daq.txt
-- Up-to-date: /usr/local/share/doc/snort/dcerpc.txt
-- Up-to-date: /usr/local/share/doc/snort/errors.txt
-- Up-to-date: /usr/local/share/doc/snort/extractor.txt
-- Up-to-date: /usr/local/share/doc/snort/features.txt
-- Up-to-date: /usr/local/share/doc/snort/file_processing.txt
-- Up-to-date: /usr/local/share/doc/snort/ftp.txt
-- Up-to-date: /usr/local/share/doc/snort/high_availability.txt
-- Up-to-date: /usr/local/share/doc/snort/http_inspect.txt
-- Up-to-date: /usr/local/share/doc/snort/http2_inspect.txt
-- Up-to-date: /usr/local/share/doc/snort/iec104.txt
-- Up-to-date: /usr/local/share/doc/snort/js_norm.txt
-- Up-to-date: /usr/local/share/doc/snort/mms.txt
-- Up-to-date: /usr/local/share/doc/snort/opcua.txt
-- Up-to-date: /usr/local/share/doc/snort/overview.txt
-- Up-to-date: /usr/local/share/doc/snort/params.txt
-- Up-to-date: /usr/local/share/doc/snort/perf_monitor.txt
-- Up-to-date: /usr/local/share/doc/snort/pop_imap.txt
-- Up-to-date: /usr/local/share/doc/snort/port_scan.txt
-- Up-to-date: /usr/local/share/doc/snort/sensitive_data.txt
-- Up-to-date: /usr/local/share/doc/snort/side_channel.txt
-- Up-to-date: /usr/local/share/doc/snort/smtp.txt
-- Up-to-date: /usr/local/share/doc/snort/snort2x.png
-- Up-to-date: /usr/local/share/doc/snort/snort3x.png
-- Up-to-date: /usr/local/share/doc/snort/snort_user.txt
-- Up-to-date: /usr/local/share/doc/snort/snorty.png
-- Up-to-date: /usr/local/share/doc/snort/telnet.txt
-- Up-to-date: /usr/local/share/doc/snort/terms.txt
-- Up-to-date: /usr/local/share/doc/snort/trace.txt
-- Up-to-date: /usr/local/share/doc/snort/tutorial.txt
-- Up-to-date: /usr/local/share/doc/snort/usage.txt
-- Up-to-date: /usr/local/share/doc/snort/wizard.txt
-- Up-to-date: /usr/local/share/doc/snort/snort_user.text
-- Up-to-date: /usr/local/share/doc/snort/appendix.txt
-- Up-to-date: /usr/local/share/doc/snort/building.txt
-- Up-to-date: /usr/local/share/doc/snort/builtin_stubs.txt
-- Up-to-date: /usr/local/share/doc/snort/enviro.txt
-- Up-to-date: /usr/local/share/doc/snort/snort_reference.txt
-- Up-to-date: /usr/local/share/doc/snort/snort_reference.text
-- Up-to-date: /usr/local/share/doc/snort/differences.txt
-- Up-to-date: /usr/local/share/doc/snort/overview.txt
-- Up-to-date: /usr/local/share/doc/snort/snort2lua.txt
-- Up-to-date: /usr/local/share/doc/snort/snort_upgrade.txt
-- Up-to-date: /usr/local/share/doc/snort/snort_upgrade.text
-- Up-to-date: /usr/local/share/doc/snort/snort_devel.txt
-- Up-to-date: /usr/local/share/doc/snort/extending.txt
-- Up-to-date: /usr/local/share/doc/snort/style.txt
-- Up-to-date: /usr/local/share/doc/snort/versions.txt






,,_     -*> Snort++ <*-
  o"  )~   Version 3.12.2.0
   ''''    By Martin Roesch & The Snort Team
           http://snort.org/contact#team
           Copyright (C) 2014-2026 Cisco and/or its affiliates. All rights reserved.
           Copyright (C) 1998-2013 Sourcefire, Inc., et al.
           Using DAQ version 3.0.24
           Using libpcap version 1.10.6 (64-bit time_t, with TPACKET_V3)
           Using LuaJIT version 2.1.1761786044
           Using LZMA version 5.8.3
           Using OpenSSL 3.6.3 9 Jun 2026
           Using PCRE2 version 10.46 2025-08-27
           Using ZLIB version 1.3.2








┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo ldconfig
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ snort -V

   ,,_     -*> Snort++ <*-
  o"  )~   Version 3.12.2.0
   ''''    By Martin Roesch & The Snort Team
           http://snort.org/contact#team
           Copyright (C) 2014-2026 Cisco and/or its affiliates. All rights reserved.
           Copyright (C) 1998-2013 Sourcefire, Inc., et al.
           Using DAQ version 3.0.27
           Using libpcap version 1.10.6 (64-bit time_t, with TPACKET_V3)
           Using LuaJIT version 2.1.1761786044
           Using LZMA version 5.8.3
           Using OpenSSL 3.6.3 9 Jun 2026
           Using PCRE2 version 10.46 2025-08-27
           Using ZLIB version 1.3.2









┌──(kali㉿kali)-[~]
└─$ sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install -y build-essential libpcre3-dev libdumbnet-dev bison flex zlib1g-dev liblzma-dev libssl-dev libluajit-5.1-dev pkg-config libhwloc-dev cmake libpcap-dev libunwind-dev git

[sudo] password for kali: 
Hit:1 http://http.kali.org/kali kali-rolling InRelease 
Reading package lists... Done                          
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Calculating upgrade... Done
The following packages were automatically installed and are no longer required:
  aardvark-dns buildah catatonit conmon containers-storage crun
  docker-compose fuse-overlayfs golang-github-containers-common
  golang-github-containers-image gvproxy libblake3-0 libcriu2 libslirp0
  libsubid5 netavark passt podman slirp4netns uidmap
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
build-essential is already the newest version (12.12).
build-essential set to manually installed.
flex is already the newest version (2.6.4-8.2+b5).
flex set to manually installed.
zlib1g-dev is already the newest version (1:1.3.dfsg+really1.3.2-3).
zlib1g-dev set to manually installed.
liblzma-dev is already the newest version (5.8.3-1).
liblzma-dev set to manually installed.
git is already the newest version (1:2.53.0-1).
git set to manually installed.
Solving dependencies... Done
The following packages were automatically installed and are no longer required:
  aardvark-dns buildah catatonit conmon containers-storage crun
  docker-compose fuse-overlayfs golang-github-containers-common
  golang-github-containers-image gvproxy libblake3-0 libcriu2 libslirp0
  libsubid5 netavark passt podman slirp4netns uidmap
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  autoconf automake autotools-dev libdbus-1-dev libltdl-dev libnuma-dev
  libpcap0.8-dev libpcre16-3 libpcre32-3 libpcrecpp0v5 libpkgconf7
  librhash1 libsystemd-dev libtool pkgconf pkgconf-bin
Suggested packages:
  autoconf-archive gnu-standards autoconf-doc gettext bison-doc cmake-doc
  cmake-format elpa-cmake-mode ninja-build libtool-doc libssl-doc
  gfortran | fortran95-compiler
The following NEW packages will be installed:
  autoconf automake autotools-dev bison cmake libdbus-1-dev
  libdumbnet-dev libhwloc-dev libltdl-dev libluajit-5.1-dev libnuma-dev
  libpcap-dev libpcap0.8-dev libpcre16-3 libpcre3-dev libpcre32-3
  libpcrecpp0v5 libpkgconf7 librhash1 libssl-dev libsystemd-dev libtool
  libunwind-dev pkg-config pkgconf pkgconf-bin
0 upgraded, 26 newly installed, 0 to remove and 0 not upgraded.
Need to get 27.2 MB of archives.
After this operation, 106 MB of additional disk space will be used.
Get:1 http://kali.download/kali kali-rolling/main amd64 autoconf all 2.73-2 [516 kB]
Get:2 http://http.kali.org/kali kali-rolling/main amd64 autotools-dev all 20240727.1+nmu1 [60.0 kB]
Get:3 http://kali.download/kali kali-rolling/main amd64 automake all 1:1.18.1-4 [877 kB]
Get:4 http://http.kali.org/kali kali-rolling/main amd64 bison amd64 2:3.8.2+dfsg-1+b3 [1,170 kB]
Get:5 http://http.kali.org/kali kali-rolling/main amd64 librhash1 amd64 1.4.6-1.1+b1 [135 kB]
Get:6 http://kali.download/kali kali-rolling/main amd64 cmake amd64 4.3.4-1 [16.2 MB]
Get:7 http://kali.download/kali kali-rolling/main amd64 libsystemd-dev amd64 261.1-2 [1,370 kB]
Get:8 http://kali.download/kali kali-rolling/main amd64 libpkgconf7 amd64 2.5.1-4 [47.8 kB]
Get:9 http://kali.download/kali kali-rolling/main amd64 pkgconf-bin amd64 2.5.1-4 [35.9 kB]
Get:10 http://kali.download/kali kali-rolling/main amd64 pkgconf amd64 2.5.1-4 [33.6 kB]
Get:11 http://http.kali.org/kali kali-rolling/main amd64 libdbus-1-dev amd64 1.16.2-5+b1 [213 kB]
Get:12 http://kali.download/kali kali-rolling/main amd64 libdumbnet-dev amd64 1.18.2-1 [63.5 kB]
Get:13 http://http.kali.org/kali kali-rolling/main amd64 libnuma-dev amd64 2.0.19-1+b2 [36.2 kB]
Get:14 http://kali.download/kali kali-rolling/main amd64 libltdl-dev amd64 2.5.4-11 [168 kB]
Get:15 http://kali.download/kali kali-rolling/main amd64 libhwloc-dev amd64 2.14.0-2 [260 kB]
Get:16 http://http.kali.org/kali kali-rolling/main amd64 libluajit-5.1-dev amd64 2.1.0+openresty20251030-1+b2 [288 kB]
Get:17 http://kali.download/kali kali-rolling/main amd64 libpcap0.8-dev amd64 1.10.6-2 [292 kB]
Get:18 http://kali.download/kali kali-rolling/main amd64 libpcap-dev amd64 1.10.6-2 [36.4 kB]
Get:19 http://kali.download/kali kali-rolling/main amd64 libpcre16-3 amd64 2:8.39-15.1 [263 kB]
Get:20 http://kali.download/kali kali-rolling/main amd64 libpcre32-3 amd64 2:8.39-15.1 [251 kB]
Get:21 http://kali.download/kali kali-rolling/main amd64 libpcrecpp0v5 amd64 2:8.39-15.1 [143 kB]
Get:22 http://kali.download/kali kali-rolling/main amd64 libpcre3-dev amd64 2:8.39-15.1 [671 kB]
Get:23 http://kali.download/kali kali-rolling/main amd64 libssl-dev amd64 3.6.3-1 [3,025 kB]
Get:24 http://kali.download/kali kali-rolling/main amd64 libtool all 2.5.4-11 [539 kB]
Get:25 http://kali.download/kali kali-rolling/main amd64 libunwind-dev amd64 1.8.1-0.4 [481 kB]
Get:26 http://kali.download/kali kali-rolling/main amd64 pkg-config amd64 2.5.1-4 [18.1 kB]
Fetched 27.2 MB in 38s (713 kB/s)                                         
Selecting previously unselected package autoconf.
(Reading database… 435705 files and directories currently installed.)
Preparing to unpack …/00-autoconf_2.73-2_all.deb…
Unpacking autoconf (2.73-2)…
Selecting previously unselected package autotools-dev.
Preparing to unpack …/01-autotools-dev_20240727.1+nmu1_all.deb…
Unpacking autotools-dev (20240727.1+nmu1)…
Selecting previously unselected package automake.
Preparing to unpack …/02-automake_1%3a1.18.1-4_all.deb…
Unpacking automake (1:1.18.1-4)…
Selecting previously unselected package bison.
Preparing to unpack …/03-bison_2%3a3.8.2+dfsg-1+b3_amd64.deb…
Unpacking bison (2:3.8.2+dfsg-1+b3)…
Selecting previously unselected package librhash1:amd64.
Preparing to unpack …/04-librhash1_1.4.6-1.1+b1_amd64.deb…
Unpacking librhash1:amd64 (1.4.6-1.1+b1)…
Selecting previously unselected package cmake.
Preparing to unpack …/05-cmake_4.3.4-1_amd64.deb…
Unpacking cmake (4.3.4-1)…
Selecting previously unselected package libsystemd-dev:amd64.
Preparing to unpack …/06-libsystemd-dev_261.1-2_amd64.deb…
Unpacking libsystemd-dev:amd64 (261.1-2)…
Selecting previously unselected package libpkgconf7:amd64.
Preparing to unpack …/07-libpkgconf7_2.5.1-4_amd64.deb…
Unpacking libpkgconf7:amd64 (2.5.1-4)…
Selecting previously unselected package pkgconf-bin.
Preparing to unpack …/08-pkgconf-bin_2.5.1-4_amd64.deb…
Unpacking pkgconf-bin (2.5.1-4)…
Selecting previously unselected package pkgconf:amd64.
Preparing to unpack …/09-pkgconf_2.5.1-4_amd64.deb…
Unpacking pkgconf:amd64 (2.5.1-4)…
Selecting previously unselected package libdbus-1-dev:amd64.
Preparing to unpack …/10-libdbus-1-dev_1.16.2-5+b1_amd64.deb…
Unpacking libdbus-1-dev:amd64 (1.16.2-5+b1)…
Selecting previously unselected package libdumbnet-dev.
Preparing to unpack …/11-libdumbnet-dev_1.18.2-1_amd64.deb…
Unpacking libdumbnet-dev (1.18.2-1)…
Selecting previously unselected package libnuma-dev:amd64.
Preparing to unpack …/12-libnuma-dev_2.0.19-1+b2_amd64.deb…
Unpacking libnuma-dev:amd64 (2.0.19-1+b2)…
Selecting previously unselected package libltdl-dev:amd64.
Preparing to unpack …/13-libltdl-dev_2.5.4-11_amd64.deb…
Unpacking libltdl-dev:amd64 (2.5.4-11)…
Selecting previously unselected package libhwloc-dev:amd64.
Preparing to unpack …/14-libhwloc-dev_2.14.0-2_amd64.deb…
Unpacking libhwloc-dev:amd64 (2.14.0-2)…
Selecting previously unselected package libluajit-5.1-dev:amd64.
Preparing to unpack …/15-libluajit-5.1-dev_2.1.0+openresty20251030-1+b2_amd64.deb…
Unpacking libluajit-5.1-dev:amd64 (2.1.0+openresty20251030-1+b2)…
Selecting previously unselected package libpcap0.8-dev:amd64.
Preparing to unpack …/16-libpcap0.8-dev_1.10.6-2_amd64.deb…
Unpacking libpcap0.8-dev:amd64 (1.10.6-2)…
Selecting previously unselected package libpcap-dev:amd64.
Preparing to unpack …/17-libpcap-dev_1.10.6-2_amd64.deb…
Unpacking libpcap-dev:amd64 (1.10.6-2)…
Selecting previously unselected package libpcre16-3:amd64.
Preparing to unpack …/18-libpcre16-3_2%3a8.39-15.1_amd64.deb…
Unpacking libpcre16-3:amd64 (2:8.39-15.1)…
Selecting previously unselected package libpcre32-3:amd64.
Preparing to unpack …/19-libpcre32-3_2%3a8.39-15.1_amd64.deb…
Unpacking libpcre32-3:amd64 (2:8.39-15.1)…
Selecting previously unselected package libpcrecpp0v5:amd64.
Preparing to unpack …/20-libpcrecpp0v5_2%3a8.39-15.1_amd64.deb…
Unpacking libpcrecpp0v5:amd64 (2:8.39-15.1)…
Selecting previously unselected package libpcre3-dev:amd64.
Preparing to unpack …/21-libpcre3-dev_2%3a8.39-15.1_amd64.deb…
Unpacking libpcre3-dev:amd64 (2:8.39-15.1)…
Selecting previously unselected package libssl-dev:amd64.
Preparing to unpack …/22-libssl-dev_3.6.3-1_amd64.deb…
Unpacking libssl-dev:amd64 (3.6.3-1)…
Selecting previously unselected package libtool.
Preparing to unpack …/23-libtool_2.5.4-11_all.deb…
Unpacking libtool (2.5.4-11)…
Selecting previously unselected package libunwind-dev:amd64.
Preparing to unpack …/24-libunwind-dev_1.8.1-0.4_amd64.deb…
Unpacking libunwind-dev:amd64 (1.8.1-0.4)…
Selecting previously unselected package pkg-config:amd64.
Preparing to unpack …/25-pkg-config_2.5.1-4_amd64.deb…
Unpacking pkg-config:amd64 (2.5.1-4)…
Setting up libpcrecpp0v5:amd64 (2:8.39-15.1)…
Setting up libunwind-dev:amd64 (1.8.1-0.4)…
Setting up libpcre16-3:amd64 (2:8.39-15.1)…
Setting up libpkgconf7:amd64 (2.5.1-4)…
Setting up libnuma-dev:amd64 (2.0.19-1+b2)…
Setting up autotools-dev (20240727.1+nmu1)…
Setting up libssl-dev:amd64 (3.6.3-1)…
Setting up libpcre32-3:amd64 (2:8.39-15.1)…
Setting up pkgconf-bin (2.5.1-4)…
Setting up autoconf (2.73-2)…
Setting up libluajit-5.1-dev:amd64 (2.1.0+openresty20251030-1+b2)…
Setting up libdumbnet-dev (1.18.2-1)…
Setting up bison (2:3.8.2+dfsg-1+b3)…
update-alternatives: using /usr/bin/bison.yacc to provide /usr/bin/yacc (yacc) in auto mode
Setting up librhash1:amd64 (1.4.6-1.1+b1)…
Setting up libsystemd-dev:amd64 (261.1-2)…
Setting up automake (1:1.18.1-4)…
update-alternatives: using /usr/bin/automake-1.18 to provide /usr/bin/automake (automake) in auto mode
Setting up libtool (2.5.4-11)…
Setting up libpcre3-dev:amd64 (2:8.39-15.1)…
Setting up pkgconf:amd64 (2.5.1-4)…
Setting up libltdl-dev:amd64 (2.5.4-11)…
Setting up libdbus-1-dev:amd64 (1.16.2-5+b1)…
Setting up pkg-config:amd64 (2.5.1-4)…
Setting up cmake (4.3.4-1)…
Setting up libhwloc-dev:amd64 (2.14.0-2)…
Processing triggers for doc-base (0.11.2)…
Processing 1 added doc-base file...
Processing triggers for libc-bin (2.42-16)…
Processing triggers for man-db (2.13.1-1)…
Processing triggers for sgml-base (1.31+nmu1)…
Processing triggers for kali-menu (2026.3.2)…
Setting up libpcap0.8-dev:amd64 (1.10.6-2)…
Setting up libpcap-dev:amd64 (1.10.6-2)…
Scanning processes...                                                      
Scanning linux images...                                                   

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
                                                                           
┌──(kali㉿kali)-[~]
└─$ mkdir ~/snort_src && cd ~/snort_src

                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ wget https://snort.org
tar -xvzf libdaq-3.x.x.tar.gz
cd libdaq-3.x.x

--2026-07-22 12:26:32--  https://snort.org/
Resolving snort.org (snort.org)... 104.16.92.19, 104.16.91.19, 2606:4700::6810:5c13, ...
Connecting to snort.org (snort.org)|104.16.92.19|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: unspecified [text/html]
Saving to: ‘index.html’

index.html             [  <=>           ]  27.71K  98.7KB/s    in 0.3s    

2026-07-22 12:26:39 (98.7 KB/s) - ‘index.html’ saved [28380]

tar (child): libdaq-3.x.x.tar.gz: Cannot open: No such file or directory
tar (child): Error is not recoverable: exiting now
tar: Child returned status 2
tar: Error is not recoverable: exiting now
cd: no such file or directory: libdaq-3.x.x
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ pwd
ls -la
/home/kali/snort_src
total 36
drwxrwxr-x  2 kali kali  4096 Jul 22 12:26 .
drwx------ 23 kali kali  4096 Jul 22 12:26 ..
-rw-rw-r--  1 kali kali 28380 Jul 22 12:26 index.html
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ rm ~/snort_src/index.html
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ cd ~/snort_src
git clone https://github.com/snort3/snort3.git
Cloning into 'snort3'...
remote: Enumerating objects: 128096, done.
remote: Counting objects: 100% (13032/13032), done.
remote: Compressing objects: 100% (1947/1947), done.
error: RPC failed; curl 92 HTTP/2 stream 5 reset by server (error 0x8 CANCEL)
error: 3760 bytes of body are still expected
fetch-pack: unexpected disconnect while reading sideband packet
fatal: early EOF
fatal: fetch-pack: invalid index-pack output
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ git config --global http.version HTTP/1.1
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ cd ~/snort_src
git clone https://github.com/snort3/snort3.git
Cloning into 'snort3'...
remote: Enumerating objects: 128096, done.
remote: Counting objects: 100% (13032/13032), done.
remote: Compressing objects: 100% (1947/1947), done.
error: RPC failed; curl 18 transfer closed with outstanding read data remaining
error: 10850 bytes of body are still expected
fetch-pack: unexpected disconnect while reading sideband packet
fatal: early EOF
fatal: fetch-pack: invalid index-pack output
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ ping -c 10 github.com
PING github.com (140.82.121.3) 56(84) bytes of data.
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=1 ttl=43 time=222 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=2 ttl=43 time=223 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=3 ttl=43 time=207 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=4 ttl=43 time=206 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=5 ttl=43 time=213 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=6 ttl=43 time=212 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=7 ttl=43 time=199 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=8 ttl=43 time=199 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=9 ttl=43 time=198 ms
64 bytes from lb-140-82-121-3-fra.github.com (140.82.121.3): icmp_seq=10 ttl=43 time=212 ms

--- github.com ping statistics ---
10 packets transmitted, 10 received, 0% packet loss, time 9013ms
rtt min/avg/max/mdev = 197.794/209.117/222.940/8.682 ms
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ curl -I https://github.com
HTTP/2 200 
date: Wed, 22 Jul 2026 17:02:16 GMT
content-type: text/html; charset=utf-8
vary: X-PJAX, X-PJAX-Container, Turbo-Visit, Turbo-Frame, X-Requested-With, Accept-Language, Sec-Fetch-Site,Accept-Encoding, Accept, X-Requested-With
content-language: en-US
etag: W/"67b385aa1a2c622915137e5b576a81ae"
cache-control: max-age=0, private, must-revalidate
strict-transport-security: max-age=31536000; includeSubdomains; preload
x-frame-options: deny
x-content-type-options: nosniff
x-xss-protection: 0
referrer-policy: origin-when-cross-origin, strict-origin-when-cross-origin
content-security-policy: default-src 'none'; base-uri 'self'; child-src github.githubassets.com github.com/assets-cdn/worker/ github.com/assets/ gist.github.com/assets-cdn/worker/; connect-src 'self' uploads.github.com www.githubstatus.com collector.github.com raw.githubusercontent.com api.github.com github-cloud.s3.amazonaws.com github-production-repository-file-5c1aeb.s3.amazonaws.com github-production-upload-manifest-file-7fdce7.s3.amazonaws.com github-production-user-asset-6210df.s3.amazonaws.com *.rel.tunnels.api.visualstudio.com wss://*.rel.tunnels.api.visualstudio.com github.githubassets.com objects-origin.githubusercontent.com copilot-proxy.githubusercontent.com proxy.individual.githubcopilot.com proxy.business.githubcopilot.com proxy.enterprise.githubcopilot.com *.actions.githubusercontent.com wss://*.actions.githubusercontent.com productionresultssa0.blob.core.windows.net productionresultssa1.blob.core.windows.net productionresultssa2.blob.core.windows.net productionresultssa3.blob.core.windows.net productionresultssa4.blob.core.windows.net productionresultssa5.blob.core.windows.net productionresultssa6.blob.core.windows.net productionresultssa7.blob.core.windows.net productionresultssa8.blob.core.windows.net productionresultssa9.blob.core.windows.net productionresultssa10.blob.core.windows.net productionresultssa11.blob.core.windows.net productionresultssa12.blob.core.windows.net productionresultssa13.blob.core.windows.net productionresultssa14.blob.core.windows.net productionresultssa15.blob.core.windows.net productionresultssa16.blob.core.windows.net productionresultssa17.blob.core.windows.net productionresultssa18.blob.core.windows.net productionresultssa19.blob.core.windows.net github-production-repository-image-32fea6.s3.amazonaws.com github-production-release-asset-2e65be.s3.amazonaws.com insights.github.com wss://alive.github.com wss://alive-staging.github.com api.githubcopilot.com api.individual.githubcopilot.com api.business.githubcopilot.com api.enterprise.githubcopilot.com wss://production-copilot-host.webpubsub.azure.com edge.fullstory.com rs.fullstory.com; font-src github.githubassets.com; form-action 'self' github.com gist.github.com copilot-workspace.githubnext.com objects-origin.githubusercontent.com; frame-ancestors 'none'; frame-src viewscreen.githubusercontent.com notebooks.githubusercontent.com www.youtube-nocookie.com; img-src 'self' data: blob: github.githubassets.com media.githubusercontent.com camo.githubusercontent.com identicons.github.com avatars.githubusercontent.com private-avatars.githubusercontent.com github-cloud.s3.amazonaws.com objects.githubusercontent.com release-assets.githubusercontent.com secured-user-images.githubusercontent.com user-images.githubusercontent.com private-user-images.githubusercontent.com opengraph.githubassets.com marketplace-screenshots.githubusercontent.com copilotprodattachments.blob.core.windows.net/github-production-copilot-attachments/ github-production-user-asset-6210df.s3.amazonaws.com customer-stories-feed.github.com spotlights-feed.github.com explore-feed.github.com objects-origin.githubusercontent.com *.githubusercontent.com images.ctfassets.net/8aevphvgewt8/; manifest-src 'self'; media-src github.com user-images.githubusercontent.com secured-user-images.githubusercontent.com private-user-images.githubusercontent.com github-production-user-asset-6210df.s3.amazonaws.com gist.github.com github.githubassets.com assets.ctfassets.net/8aevphvgewt8/ videos.ctfassets.net/8aevphvgewt8/; script-src github.githubassets.com; style-src 'unsafe-inline' github.githubassets.com; upgrade-insecure-requests; worker-src github.githubassets.com github.com/assets-cdn/worker/ github.com/assets/ gist.github.com/assets-cdn/worker/
server: github.com
accept-ranges: bytes
set-cookie: _gh_sess=bJlxHdpn1jCjuYrBLcbslt%2FPN%2Fxutpmw6bCNdWxlDfHDx6Ljtp8%2FwuHjmGGZR%2BVxT1PTS4MeIz58BtYsA9tn3sUH9%2BNYtoEtnthw%2FSdva2wB%2FXUAGOXFEzOxrR%2FH8faS3VcRtK3o4564p3FmBwjjkwBhsoQ5rB4w7Jmz4CLP%2Ba80giaUqSoZUTJ7bk7V3IFH51hk7rQLlKOss8ILT5kfojoWq5h4bt1RFHZstABwH%2BJtrx2jUMeJfq6YkfWCECVffF%2Ba9moyXdDRZojKXEcnww%3D%3D--uqqlwgvWbma1u1%2Bl--YaYo7F6KMtdMzr6TGUaciw%3D%3D; path=/; HttpOnly; secure; SameSite=Lax
set-cookie: _octo=GH1.1.211285505.1784739745; expires=Thu, 22 Jul 2027 17:02:25 GMT; domain=.github.com; path=/; secure; SameSite=Lax
set-cookie: logged_in=no; expires=Thu, 22 Jul 2027 17:02:25 GMT; domain=.github.com; path=/; HttpOnly; secure; SameSite=Lax
x-github-request-id: E3E2:138D68:AE1E6B1:8EB8093:6A60F79E

                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ git config --global --get http.version
HTTP/1.1
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ rm -rf ~/snort_src/snort3
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ git clone --depth=1 https://github.com/snort3/snort3.git
Cloning into 'snort3'...
remote: Enumerating objects: 2815, done.
remote: Counting objects: 100% (2815/2815), done.
remote: Compressing objects: 100% (2116/2116), done.
remote: Total 2815 (delta 878), reused 1924 (delta 697), pack-reused 0 (from 0)
Receiving objects: 100% (2815/2815), 4.74 MiB | 14.00 KiB/s, done.
Resolving deltas: 100% (878/878), done.
                                                                           
┌──(kali㉿kali)-[~/snort_src]
└─$ cd ~/snort_src/snort3
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3]
└─$ ls                                  
ChangeLog.md              config.cmake.h.in   daqs     README.md
cmake                     configure_cmake.sh  doc      snort.pc.in
CMakeLists.txt            COPYING             LICENSE  src
cmake_uninstall.cmake.in  crusty.cfg          lua      tools
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3]
└─$ mkdir build
cd build
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ cmake ..
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- The CXX compiler identification is GNU 15.3.0
-- The C compiler identification is GNU 15.3.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Found PkgConfig: /usr/bin/pkg-config (found version "2.5.1")
-- Checking for module 'libdaq>=3.0.27'
--   Package 'libdaq' not found
CMake Error at /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:290 (message):                                                        
  Could NOT find DAQ (missing: DAQ_LIBRARIES DAQ_INCLUDE_DIR)              
Call Stack (most recent call first):                                       
  /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:654 (_FPHSA_FAILURE_MESSAGE)                                                       
  cmake/FindDAQ.cmake:34 (find_package_handle_standard_args)               
  cmake/include_libraries.cmake:4 (find_package)                           
  CMakeLists.txt:30 (include)                                              
                                                                           
                                                                           
-- Configuring incomplete, errors occurred!
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ pkg-config --modversion libdaq
Package libdaq was not found in the pkg-config search path.
Perhaps you should add the directory containing `libdaq.pc'
to the PKG_CONFIG_PATH environment variable
Package 'libdaq' not found
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ find /usr /usr/local -name "libdaq*" 2>/dev/null
/usr/share/doc/libdaq3
/usr/lib/x86_64-linux-gnu/libdaq.so.3
/usr/lib/x86_64-linux-gnu/libdaq.so.3.0.0
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ dpkg -l | grep libdaq
ii  libdaq3                                3.0.24-0kali1                            amd64        Data Acquisition library for packet I/O - shared library
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo apt update
sudo apt install libdaq-dev
[sudo] password for kali: 
Hit:1 http://http.kali.org/kali kali-rolling InRelease
All packages are up to date.    
The following packages were automatically installed and are no longer required:
  aardvark-dns        fuse-overlayfs                   libsubid5
  buildah             golang-github-containers-common  netavark
  catatonit           golang-github-containers-image   passt
  conmon              gvproxy                          podman
  containers-storage  libblake3-0                      slirp4netns
  crun                libcriu2                         uidmap
  docker-compose      libslirp0
Use 'sudo apt autoremove' to remove them.

Installing:
  libdaq-dev
                                                                           
Installing dependencies:
  libdaq2  libnetfilter-queue-dev  libnfnetlink-dev
                                                                           
Suggested packages:
  libnetfilter-queue-doc

Summary:
  Upgrading: 0, Installing: 4, Removing: 0, Not Upgrading: 0
  Download size: 224 kB
  Space needed: 919 kB / 54.5 GB available

Continue? [Y/n] Y
Get:1 http://http.kali.org/kali kali-rolling/main amd64 libdaq2 amd64 3.0.12+really2.0.7-0kali3 [86.6 kB]
Get:2 http://http.kali.org/kali kali-rolling/main amd64 libnfnetlink-dev amd64 1.0.2-3+b2 [8,220 B]
Get:3 http://http.kali.org/kali kali-rolling/main amd64 libnetfilter-queue-dev amd64 1.0.5-4+b2 [18.5 kB]
Get:4 http://http.kali.org/kali kali-rolling/main amd64 libdaq-dev amd64 3.0.12+really2.0.7-0kali3 [110 kB]
Fetched 224 kB in 7s (30.2 kB/s)                  
Selecting previously unselected package libdaq2.
(Reading database… 441866 files and directories currently installed.)
Preparing to unpack …/libdaq2_3.0.12+really2.0.7-0kali3_amd64.deb…
Unpacking libdaq2 (3.0.12+really2.0.7-0kali3)…
Selecting previously unselected package libnfnetlink-dev:amd64.
Preparing to unpack …/libnfnetlink-dev_1.0.2-3+b2_amd64.deb…
Unpacking libnfnetlink-dev:amd64 (1.0.2-3+b2)…
Selecting previously unselected package libnetfilter-queue-dev:amd64.
Preparing to unpack …/libnetfilter-queue-dev_1.0.5-4+b2_amd64.deb…
Unpacking libnetfilter-queue-dev:amd64 (1.0.5-4+b2)…
Selecting previously unselected package libdaq-dev.
Preparing to unpack …/libdaq-dev_3.0.12+really2.0.7-0kali3_amd64.deb…
Unpacking libdaq-dev (3.0.12+really2.0.7-0kali3)…
Setting up libnfnetlink-dev:amd64 (1.0.2-3+b2)…
Setting up libnetfilter-queue-dev:amd64 (1.0.5-4+b2)…
Setting up libdaq2 (3.0.12+really2.0.7-0kali3)…
Setting up libdaq-dev (3.0.12+really2.0.7-0kali3)…
Processing triggers for libc-bin (2.42-16)…
Processing triggers for kali-menu (2026.3.2)…
Scanning processes...                                                      
Scanning linux images...                                                   

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ find /usr -name "libdaq.pc" 2>/dev/null
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ find /usr -name "libdaq.pc" 2>/dev/null
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ dpkg -L libdaq-dev | grep -E "daq|pc"
/usr/bin/daq-modules-config
/usr/include/daq.h
/usr/include/daq_api.h
/usr/include/daq_common.h
/usr/lib/x86_64-linux-gnu/libdaq.a
/usr/lib/x86_64-linux-gnu/libdaq_static.a
/usr/lib/x86_64-linux-gnu/libdaq_static_modules.a
/usr/share/doc/libdaq-dev
/usr/share/doc/libdaq-dev/changelog.Debian.gz
/usr/share/doc/libdaq-dev/changelog.gz
/usr/share/doc/libdaq-dev/copyright
/usr/lib/x86_64-linux-gnu/libdaq.so
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ cd ~/snort_src/snort3/build
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ rm -rf *
zsh: sure you want to delete all 2 files in /home/kali/snort_src/snort3/build [yn]? y
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ cmake .. -DDAQ_INCLUDE_DIR=/usr/include -DDAQ_LIBRARY=/usr/lib/x86_64-linux-gnu/libdaq.so
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- The CXX compiler identification is GNU 15.3.0
-- The C compiler identification is GNU 15.3.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Found PkgConfig: /usr/bin/pkg-config (found version "2.5.1")
-- Checking for module 'libdaq>=3.0.27'
--   Package 'libdaq' not found
-- Found DAQ: /usr/lib/x86_64-linux-gnu/libdaq.so
-- Found DNET: /usr/include
-- Found FLEX: /usr/bin/flex (found suitable version "2.6.4", minimum required is "2.6.0")
-- Checking for module 'hwloc'
--   Found hwloc, version 2.14.0
-- Found HWLOC: /usr/lib/x86_64-linux-gnu/libhwloc.so
-- Checking for module 'luajit'
--   Found luajit, version 2.1.1761786044
-- Found LuaJIT: /usr/lib/x86_64-linux-gnu/libluajit-5.1.so (found version "2.1.1761786044")
-- Found OpenSSL: /usr/lib/x86_64-linux-gnu/libcrypto.so (found suitable version "3.6.3", minimum required is "1.1.1")
-- Found PCAP: /usr/lib/x86_64-linux-gnu/libpcap.so
-- Performing Test PCAP_LINKS_SOLO
-- Performing Test PCAP_LINKS_SOLO - Success
-- Checking for module 'libpcre2'
--   Package 'libpcre2' not found
CMake Error at /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:290 (message):                                                        
                                                                           
                                                                           
        ERROR! Libpcre2 library not found.                                 
                                                                           
        Get it from http://www.pcre.org                                    
   (missing: PCRE2_INCLUDE_DIR PCRE2_LIBRARIES)                            
Call Stack (most recent call first):                                       
  /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:654 (_FPHSA_FAILURE_MESSAGE)                                                       
  cmake/FindPCRE2.cmake:24 (find_package_handle_standard_args)             
  cmake/include_libraries.cmake:11 (find_package)                          
  CMakeLists.txt:30 (include)                                              
                                                                           
                                                                           
-- Configuring incomplete, errors occurred!
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo apt install libpcre2-dev
The following packages were automatically installed and are no longer required:
  aardvark-dns        fuse-overlayfs                   libsubid5
  buildah             golang-github-containers-common  netavark
  catatonit           golang-github-containers-image   passt
  conmon              gvproxy                          podman
  containers-storage  libblake3-0                      slirp4netns
  crun                libcriu2                         uidmap
  docker-compose      libslirp0
Use 'sudo apt autoremove' to remove them.

Installing:
  libpcre2-dev
                                                                           
Installing dependencies:
  libpcre2-32-0
                                                                           
Summary:
  Upgrading: 0, Installing: 2, Removing: 0, Not Upgrading: 0
  Download size: 1,114 kB
  Space needed: 3,669 kB / 54.5 GB available

Continue? [Y/n] Y
Get:1 http://http.kali.org/kali kali-rolling/main amd64 libpcre2-32-0 amd64 10.46-1+b2 [267 kB]
Get:2 http://http.kali.org/kali kali-rolling/main amd64 libpcre2-dev amd64 10.46-1+b2 [846 kB]
Fetched 1,114 kB in 5s (240 kB/s)     
Selecting previously unselected package libpcre2-32-0:amd64.
(Reading database… 441924 files and directories currently installed.)
Preparing to unpack …/libpcre2-32-0_10.46-1+b2_amd64.deb…
Unpacking libpcre2-32-0:amd64 (10.46-1+b2)…
Selecting previously unselected package libpcre2-dev:amd64.
Preparing to unpack …/libpcre2-dev_10.46-1+b2_amd64.deb…
Unpacking libpcre2-dev:amd64 (10.46-1+b2)…
Setting up libpcre2-32-0:amd64 (10.46-1+b2)…
Setting up libpcre2-dev:amd64 (10.46-1+b2)…
Processing triggers for man-db (2.13.1-1)…
Processing triggers for kali-menu (2026.3.2)…
Processing triggers for libc-bin (2.42-16)…
Scanning processes...                                                      
Scanning linux images...                                                   

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ dpkg -l | grep pcre2
ii  libpcre2-16-0:amd64                    10.46-1+b2                               amd64        New Perl Compatible Regular Expression Library - 16 bit runtime files
ii  libpcre2-32-0:amd64                    10.46-1+b2                               amd64        New Perl Compatible Regular Expression Library - 32 bit runtime files
ii  libpcre2-8-0:amd64                     10.46-1+b2                               amd64        New Perl Compatible Regular Expression Library- 8 bit runtime files
ii  libpcre2-dev:amd64                     10.46-1+b2                               amd64        New Perl Compatible Regular Expression Library - development files
ii  libpcre2-posix3:amd64                  10.46-1+b2                               amd64        New Perl Compatible Regular Expression Library - posix-compatible runtime files
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ rm -rf *
zsh: sure you want to delete all 2 files in /home/kali/snort_src/snort3/build [yn]? y
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ cmake .. -DDAQ_INCLUDE_DIR=/usr/include -DDAQ_LIBRARY=/usr/lib/x86_64-linux-gnu/libdaq.so
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- The CXX compiler identification is GNU 15.3.0
-- The C compiler identification is GNU 15.3.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Found PkgConfig: /usr/bin/pkg-config (found version "2.5.1")
-- Checking for module 'libdaq>=3.0.27'
--   Package 'libdaq' not found
-- Found DAQ: /usr/lib/x86_64-linux-gnu/libdaq.so
-- Found DNET: /usr/include
-- Found FLEX: /usr/bin/flex (found suitable version "2.6.4", minimum required is "2.6.0")
-- Checking for module 'hwloc'
--   Found hwloc, version 2.14.0
-- Found HWLOC: /usr/lib/x86_64-linux-gnu/libhwloc.so
-- Checking for module 'luajit'
--   Found luajit, version 2.1.1761786044
-- Found LuaJIT: /usr/lib/x86_64-linux-gnu/libluajit-5.1.so (found version "2.1.1761786044")
-- Found OpenSSL: /usr/lib/x86_64-linux-gnu/libcrypto.so (found suitable version "3.6.3", minimum required is "1.1.1")
-- Found PCAP: /usr/lib/x86_64-linux-gnu/libpcap.so
-- Performing Test PCAP_LINKS_SOLO
-- Performing Test PCAP_LINKS_SOLO - Success
-- Checking for module 'libpcre2'
--   Package 'libpcre2' not found
-- Found PCRE2: /usr/include
-- Found ZLIB: /usr/lib/x86_64-linux-gnu/libz.so (found version "1.3.2")
CMake Warning (dev) at /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:493 (message):                                                
  The package name passed to find_package_handle_standard_args() (W3M) does
  not match the name of the calling package (Asciidoc).  This can lead to  
  problems in calling code that expects find_package() result variables    
  (e.g., `_FOUND`) to follow a certain pattern.                            
Call Stack (most recent call first):                                       
  cmake/FindAsciidoc.cmake:34 (find_package_handle_standard_args)          
  cmake/include_libraries.cmake:20 (find_package)                          
  CMakeLists.txt:30 (include)                                              
This warning is for project developers.  Use -Wno-dev to suppress it.      
                                                                           
-- install w3m to build all-in-one text user manual (missing: W3M_EXE) 
-- Checking for module 'libhs'
--   Package 'libhs' not found
-- Checking for module 'libsafec'
--   Package 'libsafec' not found
-- Performing Test ICONV_IS_BUILT_IN
-- Performing Test ICONV_IS_BUILT_IN - Success
-- Checking for module 'uuid'
--   Found uuid, version 2.42.2
-- Checking for module 'libunwind'
--   Found libunwind, version 1.8.1
-- Found Libunwind: /usr/lib/x86_64-linux-gnu/libunwind.so (found version "1.8.1")
-- Checking for module 'numa>=2.0.14'
--   Found numa, version 2.0.19
-- Checking for module 'libml_static>=2.0.0'
--   Package 'libml_static' not found
-- Performing Test HAS_C_HIDDEN
-- Performing Test HAS_C_HIDDEN - Success
-- Performing Test HAS_CXX_HIDDEN
-- Performing Test HAS_CXX_HIDDEN - Success
-- Looking for malloc_trim
-- Looking for malloc_trim - found
-- Looking for memrchr
-- Looking for memrchr - found
-- Looking for sigaction
-- Looking for sigaction - found
-- Looking for basename_r
-- Looking for basename_r - not found
-- Performing Test HAVE_GNU_STRERROR_R
-- Performing Test HAVE_GNU_STRERROR_R - Success
-- Looking for getrpcent
-- Looking for getrpcent - found
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of long int
-- Check size of long int - done
-- Check size of unsigned long int
-- Check size of unsigned long int - done
-- Performing Test INLINE
-- Performing Test INLINE - Success
-- Performing Test RESTRICT
-- Performing Test RESTRICT - Success
-- Looking for lzma_code in /usr/lib/x86_64-linux-gnu/liblzma.so
-- Looking for lzma_code in /usr/lib/x86_64-linux-gnu/liblzma.so - found
-- Looking for backtrace in /usr/lib/x86_64-linux-gnu/libunwind.so
-- Looking for backtrace in /usr/lib/x86_64-linux-gnu/libunwind.so - found
-- Looking for uuid_parse in /usr/lib/x86_64-linux-gnu/libuuid.so
-- Looking for uuid_parse in /usr/lib/x86_64-linux-gnu/libuuid.so - found

-------------------------------------------------------
snort version 3.12.2.0

Install options:
    prefix:     /usr/local
    includes:   /usr/local/include/snort
    plugins:    /usr/local/lib/snort

Compiler options:
    CC:             /usr/bin/cc
    CXX:            /usr/bin/c++
    CFLAGS:           -fvisibility=hidden   -DNDEBUG -g -ggdb    
    CXXFLAGS:         -fvisibility=hidden   -DNDEBUG -g -ggdb    
    EXE_LDFLAGS:        
    MODULE_LDFLAGS:     

Feature options:
    DAQ Modules:    Static ()
    libatomic:      System-provided
    Hyperscan:      OFF
    ICONV:          ON
    Libunwind:      ON
    LZMA:           ON
    RPC DB:         Built-in
    SafeC:          OFF
    TCMalloc:       OFF
    JEMalloc:       OFF
    UUID:           ON
    NUMA:           ON
    LibML:          OFF
-------------------------------------------------------

-- Configuring done (12.6s)
-- Generating done (1.1s)
CMake Warning:
  Manually-specified variables were not used by the project:               
                                                                           
    DAQ_LIBRARY                                                            
                                                                           
                                                                           
-- Build files have been written to: /home/kali/snort_src/snort3/build
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ make -j$(nproc)
[  0%] Building CXX object src/connectors/unixdomain_connector/CMakeFiles/unixdomain_connector.dir/unixdomain_connector.cc.o                          
[  0%] Building CXX object src/connectors/unixdomain_connector/CMakeFiles/unixdomain_connector.dir/unixdomain_connector_module.cc.o                   
[  0%] Built target unixdomain_connector
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/codec.cc.o                                                                          
In file included from /home/kali/snort_src/snort3/src/detection/ips_context.h:35,
                 from /home/kali/snort_src/snort3/src/detection/detection_engine.h:29,
                 from /home/kali/snort_src/snort3/src/framework/codec.cc:27:
/home/kali/snort_src/snort3/src/protocols/packet.h:155:5: error: ‘DAQ_Msg_h’ does not name a type
  155 |     DAQ_Msg_h daq_msg = nullptr;            // DAQ message this packet came from
      |     ^~~~~~~~~
/home/kali/snort_src/snort3/src/protocols/packet.h: In member function ‘bool snort::Packet::is_inter_group_flow() const’:
/home/kali/snort_src/snort3/src/protocols/packet.h:359:29: error: ‘DAQ_PKT_FLAG_SIGNIFICANT_GROUPS’ was not declared in this scope
  359 |     { return (pkth->flags & DAQ_PKT_FLAG_SIGNIFICANT_GROUPS) != 0; }
      |                             ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
make[2]: *** [src/framework/CMakeFiles/framework.dir/build.make:79: src/framework/CMakeFiles/framework.dir/codec.cc.o] Error 1
make[1]: *** [CMakeFiles/Makefile2:4420: src/framework/CMakeFiles/framework.dir/all] Error 2
make: *** [Makefile:156: all] Error 2
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ rm -rf *
zsh: sure you want to delete all 15 files in /home/kali/snort_src/snort3/build [yn]? y
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ cmake ..
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- The CXX compiler identification is GNU 15.3.0
-- The C compiler identification is GNU 15.3.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Found PkgConfig: /usr/bin/pkg-config (found version "2.5.1")
-- Checking for module 'libdaq>=3.0.27'
--   Found libdaq, version 3.0.27
-- Found DAQ: /usr/local/lib/libdaq.so
-- Checking for module 'libdaq_static_dump'
--   Found libdaq_static_dump, version 3.0.27
-- Checking for module 'libdaq_static_fst'
--   Found libdaq_static_fst, version 3.0.27
-- Checking for module 'libdaq_static_afpacket'
--   Found libdaq_static_afpacket, version 3.0.27
-- Checking for module 'libdaq_static_trace'
--   Found libdaq_static_trace, version 3.0.27
-- Checking for module 'libdaq_static_savefile'
--   Found libdaq_static_savefile, version 3.0.27
-- Checking for module 'libdaq_static_pcap'
--   Found libdaq_static_pcap, version 3.0.27
-- Checking for module 'libdaq_static_gwlb'
--   Found libdaq_static_gwlb, version 3.0.27
-- Checking for module 'libdaq_static_bpf'
--   Found libdaq_static_bpf, version 3.0.27
-- Found DNET: /usr/include
-- Found FLEX: /usr/bin/flex (found suitable version "2.6.4", minimum required is "2.6.0")
-- Checking for module 'hwloc'
--   Found hwloc, version 2.14.0
-- Found HWLOC: /usr/lib/x86_64-linux-gnu/libhwloc.so
-- Checking for module 'luajit'
--   Found luajit, version 2.1.1761786044
-- Found LuaJIT: /usr/lib/x86_64-linux-gnu/libluajit-5.1.so (found version "2.1.1761786044")
-- Found OpenSSL: /usr/lib/x86_64-linux-gnu/libcrypto.so (found suitable version "3.6.3", minimum required is "1.1.1")
-- Found PCAP: /usr/lib/x86_64-linux-gnu/libpcap.so
-- Performing Test PCAP_LINKS_SOLO
-- Performing Test PCAP_LINKS_SOLO - Success
-- Checking for module 'libpcre2'
--   Package 'libpcre2' not found
-- Found PCRE2: /usr/include
-- Found ZLIB: /usr/lib/x86_64-linux-gnu/libz.so (found version "1.3.2")
CMake Warning (dev) at /usr/share/cmake-4.3/Modules/FindPackageHandleStandardArgs.cmake:493 (message):                                                
  The package name passed to find_package_handle_standard_args() (W3M) does
  not match the name of the calling package (Asciidoc).  This can lead to  
  problems in calling code that expects find_package() result variables    
  (e.g., `_FOUND`) to follow a certain pattern.                            
Call Stack (most recent call first):                                       
  cmake/FindAsciidoc.cmake:34 (find_package_handle_standard_args)          
  cmake/include_libraries.cmake:20 (find_package)                          
  CMakeLists.txt:30 (include)                                              
This warning is for project developers.  Use -Wno-dev to suppress it.      
                                                                           
-- install w3m to build all-in-one text user manual (missing: W3M_EXE) 
-- Checking for module 'libhs'
--   Package 'libhs' not found
-- Checking for module 'libsafec'
--   Package 'libsafec' not found
-- Performing Test ICONV_IS_BUILT_IN
-- Performing Test ICONV_IS_BUILT_IN - Success
-- Checking for module 'uuid'
--   Found uuid, version 2.42.2
-- Checking for module 'libunwind'
--   Found libunwind, version 1.8.1
-- Found Libunwind: /usr/lib/x86_64-linux-gnu/libunwind.so (found version "1.8.1")
-- Checking for module 'numa>=2.0.14'
--   Found numa, version 2.0.19
-- Checking for module 'libml_static>=2.0.0'
--   Package 'libml_static' not found
-- Performing Test HAS_C_HIDDEN
-- Performing Test HAS_C_HIDDEN - Success
-- Performing Test HAS_CXX_HIDDEN
-- Performing Test HAS_CXX_HIDDEN - Success
-- Looking for malloc_trim
-- Looking for malloc_trim - found
-- Looking for memrchr
-- Looking for memrchr - found
-- Looking for sigaction
-- Looking for sigaction - found
-- Looking for basename_r
-- Looking for basename_r - not found
-- Performing Test HAVE_GNU_STRERROR_R
-- Performing Test HAVE_GNU_STRERROR_R - Success
-- Looking for getrpcent
-- Looking for getrpcent - found
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of long int
-- Check size of long int - done
-- Check size of unsigned long int
-- Check size of unsigned long int - done
-- Performing Test INLINE
-- Performing Test INLINE - Success
-- Performing Test RESTRICT
-- Performing Test RESTRICT - Success
-- Looking for lzma_code in /usr/lib/x86_64-linux-gnu/liblzma.so
-- Looking for lzma_code in /usr/lib/x86_64-linux-gnu/liblzma.so - found
-- Looking for backtrace in /usr/lib/x86_64-linux-gnu/libunwind.so
-- Looking for backtrace in /usr/lib/x86_64-linux-gnu/libunwind.so - found
-- Looking for uuid_parse in /usr/lib/x86_64-linux-gnu/libuuid.so
-- Looking for uuid_parse in /usr/lib/x86_64-linux-gnu/libuuid.so - found

-------------------------------------------------------
snort version 3.12.2.0

Install options:
    prefix:     /usr/local
    includes:   /usr/local/include/snort
    plugins:    /usr/local/lib/snort

Compiler options:
    CC:             /usr/bin/cc
    CXX:            /usr/bin/c++
    CFLAGS:           -fvisibility=hidden   -DNDEBUG -g -ggdb    
    CXXFLAGS:         -fvisibility=hidden   -DNDEBUG -g -ggdb    
    EXE_LDFLAGS:        
    MODULE_LDFLAGS:     

Feature options:
    DAQ Modules:    Static (afpacket;bpf;dump;fst;gwlb;pcap;savefile;trace)
    libatomic:      System-provided
    Hyperscan:      OFF
    ICONV:          ON
    Libunwind:      ON
    LZMA:           ON
    RPC DB:         Built-in
    SafeC:          OFF
    TCMalloc:       OFF
    JEMalloc:       OFF
    UUID:           ON
    NUMA:           ON
    LibML:          OFF
-------------------------------------------------------

-- Configuring done (11.5s)
-- Generating done (1.3s)
-- Build files have been written to: /home/kali/snort_src/snort3/build
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ make -j$(nproc)
[  0%] Building CXX object src/connectors/unixdomain_connector/CMakeFiles/unixdomain_connector.dir/unixdomain_connector.cc.o                          
[  0%] Building CXX object src/connectors/unixdomain_connector/CMakeFiles/unixdomain_connector.dir/unixdomain_connector_module.cc.o                   
[  0%] Built target unixdomain_connector
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/codec.cc.o                                                                          
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/cursor.cc.o                                                                         
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/data_bus.cc.o                                                                       
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/inspector.cc.o                                                                      
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/ips_action.cc.o                                                                     
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/ips_option.cc.o                                                                     
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/parameter.cc.o                                                                      
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/pig_pen.cc.o                                                                        
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/module.cc.o                                                                         
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/mp_data_bus.cc.o                                                                    
[  1%] Building CXX object src/framework/CMakeFiles/framework.dir/mpse.cc.o
[  2%] Building CXX object src/framework/CMakeFiles/framework.dir/mpse_batch.cc.o                                                                     
[  2%] Building CXX object src/framework/CMakeFiles/framework.dir/range.cc.o                                                                          
[  2%] Building CXX object src/framework/CMakeFiles/framework.dir/tracer.cc.o                                                                         
[  2%] Building CXX object src/framework/CMakeFiles/framework.dir/value.cc.o                                                                          
[  2%] Built target framework
[  2%] Building CXX object src/mp_transport/mp_unix_transport/CMakeFiles/mp_unix_transport.dir/mp_unix_transport.cc.o                                 
[  2%] Building CXX object src/mp_transport/mp_unix_transport/CMakeFiles/mp_unix_transport.dir/mp_unix_transport_module.cc.o                          
[  2%] Built target mp_unix_transport
[  2%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/actions_module.cc.o                                                                 
[  2%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/ips_actions.cc.o                                                                    
[  2%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_alert.cc.o                                                                      
[  2%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_block.cc.o                                                                      
[  2%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_drop.cc.o                                                                       
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_file_id.cc.o                                                                    
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_log.cc.o                                                                        
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_pass.cc.o                                                                       
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_react.cc.o                                                                      
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_reject.cc.o                                                                     
[  3%] Building CXX object src/actions/CMakeFiles/ips_actions.dir/act_replace.cc.o                                                                    
[  3%] Built target ips_actions
[  3%] Building CXX object src/codecs/CMakeFiles/codecs.dir/codec_api.cc.o
[  3%] Building CXX object src/codecs/CMakeFiles/codecs.dir/codec_module.cc.o                                                                         
[  3%] Built target codecs
[  3%] Building CXX object src/codecs/root/CMakeFiles/root_codecs.dir/cd_eth.cc.o                                                                     
[  3%] Building CXX object src/codecs/root/CMakeFiles/root_codecs.dir/cd_raw.cc.o                                                                     
[  3%] Built target root_codecs
[  3%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_arp.cc.o                                                                     
[  3%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_erspan2.cc.o                                                                 
[  3%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_erspan3.cc.o                                                                 
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_ciscometadata.cc.o                                                           
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_fabricpath.cc.o                                                              
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_mpls.cc.o                                                                    
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_ppp_encap.cc.o                                                               
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_pppoe.cc.o                                                                   
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_trans_bridge.cc.o                                                            
[  4%] Building CXX object src/codecs/link/CMakeFiles/link_codecs.dir/cd_vlan.cc.o                                                                    
[  4%] Built target link_codecs
[  4%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_ipv4.cc.o                                                                        
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_ipv6.cc.o                                                                        
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_hop_opts.cc.o                                                                    
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_tcp.cc.o                                                                         
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_auth.cc.o                                                                        
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_bad_proto.cc.o                                                                   
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_dst_opts.cc.o                                                                    
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_esp.cc.o                                                                         
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_frag.cc.o                                                                        
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_gre.cc.o                                                                         
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_icmp4.cc.o                                                                       
[  5%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_icmp6.cc.o                                                                       
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_igmp.cc.o                                                                        
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_no_next.cc.o                                                                     
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_mobility.cc.o                                                                    
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_pgm.cc.o                                                                         
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_routing.cc.o                                                                     
[  6%] Building CXX object src/codecs/ip/CMakeFiles/ip_codecs.dir/cd_udp.cc.o                                                                         
[  6%] Built target ip_codecs
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_default.cc.o                                                                 
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_gtp.cc.o                                                                     
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_icmp4_ip.cc.o                                                                
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_icmp6_ip.cc.o                                                                
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_llc.cc.o                                                                     
[  6%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_teredo.cc.o                                                                  
[  7%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_user.cc.o                                                                    
[  7%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_vxlan.cc.o                                                                   
[  7%] Building CXX object src/codecs/misc/CMakeFiles/misc_codecs.dir/cd_geneve.cc.o                                                                  
[  7%] Built target misc_codecs
[  7%] Building CXX object src/control/CMakeFiles/control.dir/control.cc.o
[  7%] Built target control
[  7%] Building CXX object src/detection/CMakeFiles/detection.dir/context_switcher.cc.o                                                               
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/detect.cc.o                                                                         
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/detection_engine.cc.o                                                               
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/detection_module.cc.o                                                               
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/detection_options.cc.o                                                              
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/detect_trace.cc.o                                                                   
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/event_trace.cc.o                                                                    
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/extract.cc.o                                                                        
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/fp_config.cc.o                                                                      
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/fp_create.cc.o                                                                      
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/fp_detect.cc.o                                                                      
[  8%] Building CXX object src/detection/CMakeFiles/detection.dir/fp_utils.cc.o                                                                       
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/ips_context.cc.o                                                                    
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/ips_context_chain.cc.o                                                              
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/ips_context_data.cc.o                                                               
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/pcrm.cc.o
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/regex_offload.cc.o                                                                  
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/rtn_checks.cc.o                                                                     
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/rules.cc.o                                                                          
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/service_map.cc.o                                                                    
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/sfrim.cc.o                                                                          
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/signature.cc.o                                                                      
[  9%] Building CXX object src/detection/CMakeFiles/detection.dir/treenodes.cc.o                                                                      
[ 10%] Building CXX object src/detection/CMakeFiles/detection.dir/tag.cc.o
[ 10%] Built target detection
[ 10%] Building CXX object src/dump_config/CMakeFiles/dump_config.dir/config_data.cc.o                                                                
[ 10%] Building CXX object src/dump_config/CMakeFiles/dump_config.dir/config_output.cc.o                                                              
[ 10%] Building CXX object src/dump_config/CMakeFiles/dump_config.dir/json_config_output.cc.o                                                         
[ 10%] Building CXX object src/dump_config/CMakeFiles/dump_config.dir/text_config_output.cc.o                                                         
[ 10%] Built target dump_config
[ 10%] Building CXX object src/events/CMakeFiles/events.dir/event.cc.o
[ 11%] Building CXX object src/events/CMakeFiles/events.dir/event_queue.cc.o                                                                          
[ 11%] Building CXX object src/events/CMakeFiles/events.dir/sfeventq.cc.o
[ 11%] Built target events
[ 11%] Building CXX object src/file_api/CMakeFiles/file_api.dir/circular_buffer.cc.o                                                                  
[ 11%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_api.cc.o                                                                         
[ 11%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_capture.cc.o                                                                     
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_cache.cc.o                                                                       
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_cache_share.cc.o                                                                 
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_config.cc.o                                                                      
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_flows.cc.o                                                                       
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_identifier.cc.o                                                                  
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_inspect.cc.o                                                                     
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_lib.cc.o                                                                         
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_log.cc.o                                                                         
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_mempool.cc.o                                                                     
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_module.cc.o                                                                      
[ 12%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_policy.cc.o                                                                      
[ 13%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_segment.cc.o                                                                     
[ 13%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_service.cc.o                                                                     
[ 13%] Building CXX object src/file_api/CMakeFiles/file_api.dir/file_stats.cc.o                                                                       
[ 13%] Built target file_api
[ 13%] Building CXX object src/filters/CMakeFiles/filter.dir/detection_filter.cc.o                                                                    
[ 13%] Building CXX object src/filters/CMakeFiles/filter.dir/rate_filter.cc.o                                                                         
[ 13%] Building CXX object src/filters/CMakeFiles/filter.dir/sfthreshold.cc.o                                                                         
[ 13%] Building CXX object src/filters/CMakeFiles/filter.dir/sfrf.cc.o
[ 13%] Building CXX object src/filters/CMakeFiles/filter.dir/sfthd.cc.o
[ 13%] Built target filter
[ 13%] Building CXX object src/flow/CMakeFiles/flow.dir/deferred_trust.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/dump_flows.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/dump_flows_serializer.cc.o                                                                    
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/expect_cache.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow_cache.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow_control.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow_data.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow_key.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/flow_stash.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/ha.cc.o
[ 14%] Building CXX object src/flow/CMakeFiles/flow.dir/ha_module.cc.o
[ 14%] Built target flow
[ 14%] Building CXX object src/hash/CMakeFiles/hash.dir/ghash.cc.o
[ 14%] Building CXX object src/hash/CMakeFiles/hash.dir/hashes.cc.o
[ 14%] Building CXX object src/hash/CMakeFiles/hash.dir/hash_lru_cache.cc.o
[ 14%] Building CXX object src/hash/CMakeFiles/hash.dir/hash_key_operations.cc.o                                                                      
[ 15%] Building CXX object src/hash/CMakeFiles/hash.dir/lru_cache_shared.cc.o                                                                         
[ 15%] Building CXX object src/hash/CMakeFiles/hash.dir/primetable.cc.o
[ 15%] Building CXX object src/hash/CMakeFiles/hash.dir/xhash.cc.o
[ 15%] Building CXX object src/hash/CMakeFiles/hash.dir/zhash.cc.o
[ 15%] Built target hash
[ 15%] [FLEX][pdf_tokenizer] Building scanner with flex 2.6.4
[ 15%] [FLEX][js_tokenizer] Building scanner with flex 2.6.4
[ 16%] Generating js_tokenizer.cc
[ 16%] Generating pdf_tokenizer.cc
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/pdf_tokenizer.cc.o                                                                      
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_tokenizer.cc.o                                                                       
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_identifier_ctx.cc.o                                                                  
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_norm.cc.o
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_norm_module.cc.o                                                                     
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_normalizer.cc.o                                                                      
[ 16%] Building CXX object src/js_norm/CMakeFiles/js_norm.dir/js_pdf_norm.cc.o                                                                        
[ 16%] Built target js_norm
[ 16%] Building CXX object src/latency/CMakeFiles/latency.dir/latency_module.cc.o                                                                     
[ 16%] Building CXX object src/latency/CMakeFiles/latency.dir/packet_latency.cc.o                                                                     
[ 16%] Building CXX object src/latency/CMakeFiles/latency.dir/rule_latency.cc.o                                                                       
[ 16%] Built target latency
[ 16%] Building CXX object src/log/CMakeFiles/log.dir/batched_logger.cc.o
[ 16%] Building CXX object src/log/CMakeFiles/log.dir/log.cc.o
[ 16%] Building CXX object src/log/CMakeFiles/log.dir/log_stats.cc.o
[ 16%] Building CXX object src/log/CMakeFiles/log.dir/log_text.cc.o
[ 17%] Building CXX object src/log/CMakeFiles/log.dir/messages.cc.o
[ 17%] Building CXX object src/log/CMakeFiles/log.dir/obfuscator.cc.o
[ 17%] Building CXX object src/log/CMakeFiles/log.dir/text_log.cc.o
[ 17%] Building CXX object src/log/CMakeFiles/log.dir/u2_packet.cc.o
[ 17%] Built target log
[ 17%] Generating lua_finalize.h
[ 17%] Generating lua_bootstrap.h
[ 17%] Building CXX object src/main/CMakeFiles/main.dir/analyzer.cc.o
[ 17%] Building CXX object src/main/CMakeFiles/main.dir/analyzer_command.cc.o                                                                         
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/help.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/modules.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/network_module.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/oops_handler.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/policy.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/process.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/reload_tracker.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/shell.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/snort.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/snort_config.cc.o
[ 18%] Building CXX object src/main/CMakeFiles/main.dir/snort_module.cc.o
[ 19%] Building CXX object src/main/CMakeFiles/main.dir/swapper.cc.o
[ 19%] Building CXX object src/main/CMakeFiles/main.dir/thread.cc.o
[ 19%] Building CXX object src/main/CMakeFiles/main.dir/thread_config.cc.o
[ 19%] Building CXX object src/main/CMakeFiles/main.dir/numa.cc.o
[ 19%] Built target main
[ 19%] Generating plugffi.lua, snort_plugin.lua
[ 19%] Generating lua_coreinit.h
[ 19%] Building CXX object src/managers/CMakeFiles/managers.dir/action_manager.cc.o                                                                   
[ 19%] Building CXX object src/managers/CMakeFiles/managers.dir/codec_manager.cc.o                                                                    
[ 19%] Building CXX object src/managers/CMakeFiles/managers.dir/connector_manager.cc.o                                                                
[ 19%] Building CXX object src/managers/CMakeFiles/managers.dir/event_manager.cc.o                                                                    
[ 19%] Building CXX object src/managers/CMakeFiles/managers.dir/inspector_manager.cc.o                                                                
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/ips_manager.cc.o                                                                      
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/module_manager.cc.o                                                                   
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/mp_transport_manager.cc.o                                                             
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/mpse_manager.cc.o                                                                     
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/plugin_manager.cc.o                                                                   
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/policy_selector_manager.cc.o                                                          
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/script_manager.cc.o                                                                   
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/so_manager.cc.o                                                                       
[ 20%] Building CXX object src/managers/CMakeFiles/managers.dir/trace_logger_manager.cc.o                                                             
[ 20%] Built target managers
[ 20%] Building CXX object src/memory/CMakeFiles/memory.dir/heap_interface.cc.o                                                                       
[ 21%] Building CXX object src/memory/CMakeFiles/memory.dir/memory_cap.cc.o
[ 21%] Building CXX object src/memory/CMakeFiles/memory.dir/memory_module.cc.o                                                                        
[ 21%] Building CXX object src/memory/CMakeFiles/memory.dir/memory_overloads.cc.o                                                                     
[ 21%] Built target memory
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_b64.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_base.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_bit.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_buffer.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_qp.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/decode_uu.cc.o
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_config.cc.o                                                                         
[ 21%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_context_data.cc.o                                                                   
[ 22%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_decode.cc.o                                                                         
[ 22%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_form_data.cc.o                                                                      
[ 22%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_log.cc.o
[ 22%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_paf.cc.o
[ 22%] Building CXX object src/mime/CMakeFiles/mime.dir/file_mime_process.cc.o                                                                        
[ 22%] Built target mime
[ 22%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/active.cc.o                                                                         
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/packet_constraints.cc.o                                                             
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/packet_tracer.cc.o                                                                  
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/packet_tracer_module.cc.o                                                           
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/sfdaq.cc.o                                                                          
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/sfdaq_config.cc.o                                                                   
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/sfdaq_instance.cc.o                                                                 
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/sfdaq_module.cc.o                                                                   
[ 23%] Building CXX object src/packet_io/CMakeFiles/packet_io.dir/trough.cc.o                                                                         
[ 23%] Built target packet_io
[ 23%] Building CXX object src/parser/CMakeFiles/parser.dir/arg_list.cc.o
[ 23%] Building CXX object src/parser/CMakeFiles/parser.dir/parser.cc.o
[ 23%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_conf.cc.o
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_ip.cc.o
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_ports.cc.o                                                                          
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_rule.cc.o
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_so_rule.cc.o                                                                        
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_stream.cc.o                                                                         
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/parse_utils.cc.o                                                                          
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/cmd_line.cc.o
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/config_file.cc.o                                                                          
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/var_dependency.cc.o                                                                       
[ 24%] Building CXX object src/parser/CMakeFiles/parser.dir/vars.cc.o
[ 24%] Built target parser
[ 24%] Building CXX object src/payload_injector/CMakeFiles/payload_injector.dir/payload_injector.cc.o                                                 
[ 25%] Building CXX object src/payload_injector/CMakeFiles/payload_injector.dir/payload_injector_module.cc.o                                          
[ 25%] Building CXX object src/payload_injector/CMakeFiles/payload_injector.dir/payload_injector_translate_page.cc.o                                  
[ 25%] Built target payload_injector
[ 25%] Building CXX object src/ports/CMakeFiles/ports.dir/port_group.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_item.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_object.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_object2.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_table.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_utils.cc.o
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/port_var_table.cc.o                                                                         
[ 26%] Building CXX object src/ports/CMakeFiles/ports.dir/rule_port_tables.cc.o                                                                       
[ 26%] Built target ports
[ 26%] Building CXX object src/protocols/CMakeFiles/protocols.dir/layer.cc.o                                                                          
[ 26%] Building CXX object src/protocols/CMakeFiles/protocols.dir/packet.cc.o                                                                         
[ 26%] Building CXX object src/protocols/CMakeFiles/protocols.dir/ip.cc.o
[ 27%] Building CXX object src/protocols/CMakeFiles/protocols.dir/ipv4_options.cc.o                                                                   
[ 27%] Building CXX object src/protocols/CMakeFiles/protocols.dir/ssl.cc.o
[ 27%] Building CXX object src/protocols/CMakeFiles/protocols.dir/tcp_options.cc.o                                                                    
[ 27%] Building CXX object src/protocols/CMakeFiles/protocols.dir/packet_manager.cc.o                                                                 
[ 27%] Built target protocols
[ 27%] Building CXX object src/sfip/CMakeFiles/sfip.dir/sf_cidr.cc.o
[ 27%] Building CXX object src/sfip/CMakeFiles/sfip.dir/sf_ip.cc.o
[ 27%] Building CXX object src/sfip/CMakeFiles/sfip.dir/sf_ipvar.cc.o
[ 27%] Building CXX object src/sfip/CMakeFiles/sfip.dir/sf_vartable.cc.o
[ 27%] Built target sfip
[ 27%] Building CXX object src/sfrt/CMakeFiles/sfrt.dir/sfrt_flat.cc.o
[ 27%] Building CXX object src/sfrt/CMakeFiles/sfrt.dir/sfrt_flat_dir.cc.o
[ 27%] Built target sfrt
[ 27%] Building CXX object src/service_inspectors/CMakeFiles/service_inspectors.dir/service_inspectors.cc.o                                           
[ 27%] Built target service_inspectors
[ 27%] Building CXX object src/service_inspectors/back_orifice/CMakeFiles/back_orifice.dir/back_orifice.cc.o                                          
[ 27%] Built target back_orifice
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/cip.cc.o                                                                     
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/cip_module.cc.o                                                              
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/cip_paf.cc.o                                                                 
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/cip_parsing.cc.o                                                             
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/cip_session.cc.o                                                             
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_attribute.cc.o                                                       
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_class.cc.o                                                           
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_connpathclass.cc.o                                                   
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_enipcommand.cc.o                                                     
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_enipreq.cc.o                                                         
[ 28%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_eniprsp.cc.o                                                         
[ 29%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_instance.cc.o                                                        
[ 29%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_req.cc.o                                                             
[ 29%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_rsp.cc.o                                                             
[ 29%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_service.cc.o                                                         
[ 29%] Building CXX object src/service_inspectors/cip/CMakeFiles/cip.dir/ips_cip_status.cc.o                                                          
[ 29%] Built target cip
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_co.cc.o                                                          
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_common.cc.o                                                      
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_context_data.cc.o                                                
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_expected_session.cc.o                                            
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_proxy.cc.o                                                  
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_proxy_module.cc.o                                           
[ 29%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_proxy_splitter.cc.o                                         
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_server.cc.o                                                 
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_server_module.cc.o                                          
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_http_server_splitter.cc.o                                        
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_list.cc.o                                                        
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb.cc.o                                                         
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb2.cc.o                                                        
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb2_commands.cc.o                                               
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb2_utils.cc.o                                                  
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_commands.cc.o                                                
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_module.cc.o                                                  
[ 30%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_paf.cc.o                                                     
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_transaction.cc.o                                             
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_transaction_utils.cc.o                                       
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_smb_utils.cc.o                                                   
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_tcp.cc.o                                                         
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_tcp_module.cc.o                                                  
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_tcp_paf.cc.o                                                     
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_udp.cc.o                                                         
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_udp_module.cc.o                                                  
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_udp_processing.cc.o                                              
[ 31%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/dce_utils.cc.o                                                       
[ 32%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/ips_dce_iface.cc.o                                                   
[ 32%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/ips_dce_opnum.cc.o                                                   
[ 32%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/ips_dce_stub_data.cc.o                                               
[ 32%] Building CXX object src/service_inspectors/dce_rpc/CMakeFiles/dce_rpc.dir/smb_message.cc.o                                                     
[ 32%] Built target dce_rpc
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/dnp3.cc.o                                                                  
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/dnp3_map.cc.o                                                              
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/dnp3_module.cc.o                                                           
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/dnp3_reassembly.cc.o                                                       
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/dnp3_paf.cc.o                                                              
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/ips_dnp3_data.cc.o                                                         
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/ips_dnp3_func.cc.o                                                         
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/ips_dnp3_ind.cc.o                                                          
[ 32%] Building CXX object src/service_inspectors/dnp3/CMakeFiles/dnp3.dir/ips_dnp3_obj.cc.o                                                          
[ 32%] Built target dnp3
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns.cc.o                                                                     
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns_config.cc.o                                                              
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns_module.cc.o                                                              
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns_rr_decoder.cc.o                                                          
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns_splitter.cc.o                                                            
[ 34%] Building CXX object src/service_inspectors/dns/CMakeFiles/dns.dir/dns_payload_event_handler.cc.o                                               
[ 34%] Built target dns
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ft_main.cc.o                                                   
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp.cc.o                                                       
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_data.cc.o                                                  
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_bounce_lookup.cc.o                                         
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_cmd_lookup.cc.o                                            
[ 34%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_module.cc.o                                                
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_parse.cc.o                                                 
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftp_print.cc.o                                                 
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/kmap.cc.o                                                      
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/telnet_splitter.cc.o                                           
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftpdata_splitter.cc.o                                          
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftpp_si.cc.o                                                   
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/ftpp_ui_config.cc.o                                            
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/pp_ftp.cc.o                                                    
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/pp_telnet.cc.o                                                 
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/telnet.cc.o                                                    
[ 35%] Building CXX object src/service_inspectors/ftp_telnet/CMakeFiles/ftp_telnet.dir/telnet_module.cc.o                                             
[ 35%] Built target ftp_telnet
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/gtp.cc.o                                                             
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/gtp_inspect.cc.o                                                     
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/gtp_module.cc.o                                                      
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/gtp_parser.cc.o                                                      
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/ips_gtp_info.cc.o                                                    
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/ips_gtp_type.cc.o                                                    
[ 36%] Building CXX object src/service_inspectors/gtp/CMakeFiles/gtp_inspect.dir/ips_gtp_version.cc.o                                                 
[ 36%] Built target gtp_inspect
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http.cc.o                                              
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_buffer_info.cc.o                                      
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_inspect.cc.o                                          
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_section.cc.o                                      
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_start.cc.o                                        
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_request.cc.o                                      
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_status.cc.o                                       
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_head_shared.cc.o                                  
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_head_shared_util.cc.o                             
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_header.cc.o                                       
[ 37%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_body.cc.o                                         
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_body_chunk.cc.o                                   
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_body_cl.cc.o                                      
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_body_hx.cc.o                                      
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_body_old.cc.o                                     
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_msg_trailer.cc.o                                      
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_query_parser.cc.o                                     
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_normalized_header.cc.o                                
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_uri.cc.o                                              
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_uri_norm.cc.o                                         
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_normalizers.cc.o                                      
[ 38%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_str_to_code.cc.o                                      
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_api.cc.o                                              
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_tables.cc.o                                           
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_module.cc.o                                           
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_test_input.cc.o                                       
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_compress_stream.cc.o                                  
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_flow_data.cc.o                                        
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_context_data.cc.o                                     
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_transaction.cc.o                                      
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_test_manager.cc.o                                     
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_field.cc.o                                            
[ 39%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_stream_splitter_finish.cc.o                           
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_stream_splitter_reassemble.cc.o                       
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_stream_splitter_scan.cc.o                             
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_cutter.cc.o                                           
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/http_js_norm.cc.o                                          
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http_buffer.cc.o                                       
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http_num_hdrs.cc.o                                     
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http_param.cc.o                                        
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http_test.cc.o                                         
[ 40%] Building CXX object src/service_inspectors/http_inspect/CMakeFiles/http_inspect.dir/ips_http_version.cc.o                                      
[ 40%] Built target http_inspect
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_api.cc.o                                           
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_data_frame.cc.o                                    
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_data_cutter.cc.o                                   
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_flow_data.cc.o                                     
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_frame.cc.o                                         
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_goaway_frame.cc.o                                  
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_headers_frame.cc.o                                 
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_headers_frame_header.cc.o                          
[ 40%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_headers_frame_trailer.cc.o                         
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_headers_frame_with_startline.cc.o                  
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_hpack.cc.o                                         
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_hpack_cookie_header_buffer.cc.o                    
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_hpack_dynamic_table.cc.o                           
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_hpack_table.cc.o                                   
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_huffman_state_machine.cc.o                         
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_inspect.cc.o                                       
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_module.cc.o                                        
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_push_promise_frame.cc.o                            
[ 41%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_request_line.cc.o                                  
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_rst_stream_frame.cc.o                              
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_settings_frame.cc.o                                
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_start_line.cc.o                                    
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_status_line.cc.o                                   
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_stream.cc.o                                        
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_stream_splitter.cc.o                               
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_stream_splitter_impl.cc.o                          
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_tables.cc.o                                        
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_utils.cc.o                                         
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/http2_window_update_frame.cc.o                           
[ 42%] Building CXX object src/service_inspectors/http2_inspect/CMakeFiles/http2_inspect.dir/ips_http2.cc.o                                           
[ 42%] Built target http2_inspect
[ 42%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104.cc.o                                                            
[ 42%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104_decode.cc.o                                                     
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104_module.cc.o                                                     
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104_paf.cc.o                                                        
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104_parse_apdu.cc.o                                                 
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/iec104_parse_information_object_elements.cc.o                          
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/ips_iec104_apci_type.cc.o                                              
[ 43%] Building CXX object src/service_inspectors/iec104/CMakeFiles/iec104.dir/ips_iec104_asdu_func.cc.o                                              
[ 43%] Built target iec104
[ 43%] Building CXX object src/service_inspectors/imap/CMakeFiles/imap.dir/imap.cc.o                                                                  
[ 43%] Building CXX object src/service_inspectors/imap/CMakeFiles/imap.dir/imap_paf.cc.o                                                              
[ 43%] Building CXX object src/service_inspectors/imap/CMakeFiles/imap.dir/imap_module.cc.o                                                           
[ 43%] Built target imap
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/mms.cc.o                                                                     
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/mms_decode.cc.o                                                              
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/mms_module.cc.o                                                              
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/mms_splitter.cc.o                                                            
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/ips_mms_data.cc.o                                                            
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/ips_mms_func.cc.o                                                            
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/tpkt/tpkt_decode.cc.o                                                        
[ 43%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/tpkt/cotp_decode.cc.o                                                        
[ 44%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/tpkt/osi_session_decode.cc.o                                                 
[ 44%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/tpkt/osi_pres_decode.cc.o                                                    
[ 44%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/tpkt/osi_acse_decode.cc.o                                                    
[ 44%] Building CXX object src/service_inspectors/mms/CMakeFiles/mms.dir/util_tpkt.cc.o                                                               
[ 44%] Built target mms
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/modbus.cc.o                                                            
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/modbus_decode.cc.o                                                     
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/modbus_module.cc.o                                                     
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/modbus_paf.cc.o                                                        
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/ips_modbus_data.cc.o                                                   
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/ips_modbus_func.cc.o                                                   
[ 44%] Building CXX object src/service_inspectors/modbus/CMakeFiles/modbus.dir/ips_modbus_unit.cc.o                                                   
[ 44%] Built target modbus
[ 44%] Building CXX object src/service_inspectors/netflow/CMakeFiles/netflow.dir/netflow_module.cc.o                                                  
[ 44%] Building CXX object src/service_inspectors/netflow/CMakeFiles/netflow.dir/netflow.cc.o                                                         
[ 44%] Built target netflow
[ 44%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/opcua.cc.o                                                               
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/opcua_decode.cc.o                                                        
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/opcua_module.cc.o                                                        
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/opcua_splitter.cc.o                                                      
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/ips_opcua_msg_type.cc.o                                                  
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/ips_opcua_msg_service.cc.o                                               
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/ips_opcua_node_id.cc.o                                                   
[ 45%] Building CXX object src/service_inspectors/opcua/CMakeFiles/opcua.dir/ips_opcua_node_namespace_index.cc.o                                      
[ 45%] Built target opcua
[ 45%] Building CXX object src/service_inspectors/pop/CMakeFiles/pop.dir/pop.cc.o                                                                     
[ 45%] Building CXX object src/service_inspectors/pop/CMakeFiles/pop.dir/pop_paf.cc.o                                                                 
[ 45%] Building CXX object src/service_inspectors/pop/CMakeFiles/pop.dir/pop_module.cc.o                                                              
[ 45%] Built target pop
[ 45%] Building CXX object src/service_inspectors/rpc_decode/CMakeFiles/rpc_decode.dir/rpc_decode.cc.o                                                
[ 45%] Building CXX object src/service_inspectors/rpc_decode/CMakeFiles/rpc_decode.dir/rpc_module.cc.o                                                
[ 45%] Built target rpc_decode
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/s7comm.cc.o                                                    
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/s7comm_decode.cc.o                                             
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/s7comm_module.cc.o                                             
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/s7comm_paf.cc.o                                                
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/ips_s7comm_content.cc.o                                        
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/ips_s7comm_func.cc.o                                           
[ 46%] Building CXX object src/service_inspectors/s7commplus/CMakeFiles/s7commplus.dir/ips_s7comm_opcode.cc.o                                         
[ 46%] Built target s7commplus
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_parser.cc.o                                                              
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_dialog.cc.o                                                              
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_utils.cc.o                                                               
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip.cc.o                                                                     
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_config.cc.o                                                              
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_module.cc.o                                                              
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/sip_splitter.cc.o                                                            
[ 46%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/ips_sip.cc.o                                                                 
[ 47%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/ips_sip_stat_code.cc.o                                                       
[ 47%] Building CXX object src/service_inspectors/sip/CMakeFiles/sip.dir/ips_sip_method.cc.o                                                          
[ 47%] Built target sip
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp.cc.o                                                                  
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp_paf.cc.o                                                              
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp_util.cc.o                                                             
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp_xlink2state.cc.o                                                      
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp_module.cc.o                                                           
[ 47%] Building CXX object src/service_inspectors/smtp/CMakeFiles/smtp.dir/smtp_normalize.cc.o                                                        
[ 47%] Built target smtp
[ 47%] Building CXX object src/service_inspectors/ssh/CMakeFiles/ssh.dir/ssh.cc.o                                                                     
[ 47%] Building CXX object src/service_inspectors/ssh/CMakeFiles/ssh.dir/ssh_module.cc.o                                                              
[ 47%] Building CXX object src/service_inspectors/ssh/CMakeFiles/ssh.dir/ssh_splitter.cc.o                                                            
[ 47%] Built target ssh
[ 47%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ips_ssl_state.cc.o                                                           
[ 47%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ips_ssl_version.cc.o                                                         
[ 47%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ssl_inspector.cc.o                                                           
[ 47%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ssl_flow_data.cc.o                                                           
[ 48%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ssl_module.cc.o                                                              
[ 48%] Building CXX object src/service_inspectors/ssl/CMakeFiles/ssl.dir/ssl_splitter.cc.o                                                            
[ 48%] Built target ssl
[ 48%] Building CXX object src/service_inspectors/tlv_pdu/CMakeFiles/tlv_pdu.dir/tlv_pdu.cc.o                                                         
[ 48%] Building CXX object src/service_inspectors/tlv_pdu/CMakeFiles/tlv_pdu.dir/tlv_pdu_splitter.cc.o                                                
[ 48%] Built target tlv_pdu
[ 48%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/curse_book.cc.o                                                        
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/dce_curse.cc.o                                                         
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/magic.cc.o                                                             
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/mms_curse.cc.o                                                         
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/opcua_curse.cc.o                                                       
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/s7commplus_curse.cc.o                                                  
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/socks_curse.cc.o                                                       
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/ssl_curse.cc.o                                                         
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/hexes.cc.o                                                             
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/spells.cc.o                                                            
[ 49%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/wizard.cc.o                                                            
[ 50%] Building CXX object src/service_inspectors/wizard/CMakeFiles/wizard.dir/wiz_module.cc.o                                                        
[ 50%] Built target wizard
[ 50%] Building CXX object src/service_inspectors/socks/CMakeFiles/socks.dir/socks_module.cc.o                                                        
[ 50%] Building CXX object src/service_inspectors/socks/CMakeFiles/socks.dir/socks.cc.o                                                               
[ 51%] Building CXX object src/service_inspectors/socks/CMakeFiles/socks.dir/socks_flow_data.cc.o                                                     
[ 51%] Building CXX object src/service_inspectors/socks/CMakeFiles/socks.dir/socks_splitter.cc.o                                                      
[ 51%] Building CXX object src/service_inspectors/socks/CMakeFiles/socks.dir/socks_ips.cc.o                                                           
[ 51%] Built target socks
[ 51%] Building CXX object src/stream/CMakeFiles/stream.dir/stream.cc.o
[ 51%] Building CXX object src/stream/CMakeFiles/stream.dir/stream_inspectors.cc.o                                                                    
[ 51%] Building CXX object src/stream/CMakeFiles/stream.dir/stream_splitter.cc.o                                                                      
[ 51%] Built target stream
[ 52%] Building CXX object src/stream/CMakeFiles/stream_paf.dir/flush_bucket.cc.o                                                                     
[ 52%] Building CXX object src/stream/CMakeFiles/stream_paf.dir/paf.cc.o
[ 52%] Building CXX object src/stream/CMakeFiles/stream_paf.dir/pafng.cc.o
[ 52%] Built target stream_paf
[ 52%] Building CXX object src/stream/base/CMakeFiles/stream_base.dir/stream_base.cc.o                                                                
[ 52%] Building CXX object src/stream/base/CMakeFiles/stream_base.dir/stream_ha.cc.o                                                                  
[ 52%] Building CXX object src/stream/base/CMakeFiles/stream_base.dir/stream_module.cc.o                                                              
[ 52%] Built target stream_base
[ 52%] Building CXX object src/stream/ip/CMakeFiles/stream_ip.dir/ip_defrag.cc.o                                                                      
[ 52%] Building CXX object src/stream/ip/CMakeFiles/stream_ip.dir/ip_ha.cc.o                                                                          
[ 52%] Building CXX object src/stream/ip/CMakeFiles/stream_ip.dir/ip_module.cc.o                                                                      
[ 52%] Building CXX object src/stream/ip/CMakeFiles/stream_ip.dir/ip_session.cc.o                                                                     
[ 52%] Building CXX object src/stream/ip/CMakeFiles/stream_ip.dir/stream_ip.cc.o                                                                      
[ 52%] Built target stream_ip
[ 52%] Building CXX object src/stream/icmp/CMakeFiles/stream_icmp.dir/icmp_ha.cc.o                                                                    
[ 52%] Building CXX object src/stream/icmp/CMakeFiles/stream_icmp.dir/icmp_module.cc.o                                                                
[ 52%] Building CXX object src/stream/icmp/CMakeFiles/stream_icmp.dir/icmp_session.cc.o                                                               
[ 52%] Building CXX object src/stream/icmp/CMakeFiles/stream_icmp.dir/stream_icmp.cc.o                                                                
[ 52%] Built target stream_icmp
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/held_packet_queue.cc.o                                                            
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/ips_stream_reassemble.cc.o                                                        
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/ips_stream_size.cc.o                                                              
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/stream_tcp.cc.o                                                                   
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_alerts.cc.o                                                                   
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_event_logger.cc.o                                                             
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_ha.cc.o                                                                       
[ 52%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_module.cc.o                                                                   
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_normalizer.cc.o                                                               
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_normalizers.cc.o                                                              
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_overlap_resolver.cc.o                                                         
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_reassembler_ids.cc.o                                                          
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_reassembler_ips.cc.o                                                          
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_reassembler.cc.o                                                              
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_reassembly_segments.cc.o                                                      
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_segment_descriptor.cc.o                                                       
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_segment_node.cc.o                                                             
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_session.cc.o                                                                  
[ 53%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_closed.cc.o                                                             
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_close_wait.cc.o                                                         
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_closing.cc.o                                                            
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_established.cc.o                                                        
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_fin_wait1.cc.o                                                          
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_fin_wait2.cc.o                                                          
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_handler.cc.o                                                            
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_last_ack.cc.o                                                           
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_listen.cc.o                                                             
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_machine.cc.o                                                            
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_mid_stream_recv.cc.o                                                    
[ 54%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_mid_stream_sent.cc.o                                                    
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_none.cc.o                                                               
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_syn_recv.cc.o                                                           
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_syn_sent.cc.o                                                           
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_state_time_wait.cc.o                                                          
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_stream_config.cc.o                                                            
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_stream_tracker.cc.o                                                           
[ 55%] Building CXX object src/stream/tcp/CMakeFiles/stream_tcp.dir/tcp_trace.cc.o                                                                    
[ 55%] Built target stream_tcp
[ 55%] Building CXX object src/stream/udp/CMakeFiles/stream_udp.dir/stream_udp.cc.o                                                                   
[ 55%] Building CXX object src/stream/udp/CMakeFiles/stream_udp.dir/udp_ha.cc.o                                                                       
[ 55%] Building CXX object src/stream/udp/CMakeFiles/stream_udp.dir/udp_module.cc.o                                                                   
[ 56%] Building CXX object src/stream/udp/CMakeFiles/stream_udp.dir/udp_session.cc.o                                                                  
[ 56%] Built target stream_udp
[ 56%] Building CXX object src/stream/user/CMakeFiles/stream_user.dir/user_module.cc.o                                                                
[ 56%] Building CXX object src/stream/user/CMakeFiles/stream_user.dir/user_session.cc.o                                                               
[ 56%] Building CXX object src/stream/user/CMakeFiles/stream_user.dir/stream_user.cc.o                                                                
[ 56%] Built target stream_user
[ 56%] Building CXX object src/stream/file/CMakeFiles/stream_file.dir/file_module.cc.o                                                                
[ 57%] Building CXX object src/stream/file/CMakeFiles/stream_file.dir/file_session.cc.o                                                               
[ 57%] Building CXX object src/stream/file/CMakeFiles/stream_file.dir/stream_file.cc.o                                                                
[ 57%] Built target stream_file
[ 57%] Building CXX object src/target_based/CMakeFiles/target_based.dir/host_attributes.cc.o                                                          
[ 57%] Building CXX object src/target_based/CMakeFiles/target_based.dir/snort_protocols.cc.o                                                          
[ 57%] Built target target_based
[ 57%] Building CXX object src/host_tracker/CMakeFiles/host_tracker.dir/cache_allocator.cc.o                                                          
[ 57%] Building CXX object src/host_tracker/CMakeFiles/host_tracker.dir/host_cache.cc.o                                                               
[ 57%] Building CXX object src/host_tracker/CMakeFiles/host_tracker.dir/host_cache_module.cc.o                                                        
[ 58%] Building CXX object src/host_tracker/CMakeFiles/host_tracker.dir/host_tracker_module.cc.o                                                      
[ 58%] Building CXX object src/host_tracker/CMakeFiles/host_tracker.dir/host_tracker.cc.o                                                             
[ 58%] Built target host_tracker
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/cip_events.cc.o                                                                         
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/detection_events.cc.o                                                                   
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/dns_events.cc.o                                                                         
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/eof_event.cc.o                                                                          
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/file_events.cc.o                                                                        
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/http_body_event.cc.o                                                                    
[ 58%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/http_events.cc.o                                                                        
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/http_form_data_event.cc.o                                                               
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/http_request_body_event.cc.o                                                            
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/http_transaction_end_event.cc.o                                                         
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/quic_events.cc.o                                                                        
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/sip_events.cc.o                                                                         
[ 59%] Building CXX object src/pub_sub/CMakeFiles/pub_sub.dir/ssh_events.cc.o                                                                         
[ 59%] Built target pub_sub
[ 60%] Building CXX object src/time/CMakeFiles/time.dir/packet_time.cc.o
[ 60%] Building CXX object src/time/CMakeFiles/time.dir/periodic.cc.o
[ 60%] Built target time
[ 60%] Building CXX object src/profiler/CMakeFiles/profiler.dir/json_view.cc.o                                                                        
[ 60%] Building CXX object src/profiler/CMakeFiles/profiler.dir/memory_context.cc.o                                                                   
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/memory_profiler.cc.o                                                                  
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/profiler.cc.o                                                                         
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/profiler_module.cc.o                                                                  
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/profiler_nodes.cc.o                                                                   
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/profiler_stats_table.cc.o                                                             
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/rule_profiler.cc.o                                                                    
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/table_view.cc.o                                                                       
[ 61%] Building CXX object src/profiler/CMakeFiles/profiler.dir/time_profiler.cc.o                                                                    
[ 61%] Built target profiler
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace.cc.o
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace_api.cc.o
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace_config.cc.o
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace_module.cc.o
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace_parser.cc.o
[ 61%] Building CXX object src/trace/CMakeFiles/trace.dir/trace_swap.cc.o
[ 61%] Built target trace
[ 61%] Building CXX object src/tracer/CMakeFiles/tracer.dir/trace_loader.cc.o                                                                         
[ 62%] Building CXX object src/tracer/CMakeFiles/tracer.dir/file_trace_logger.cc.o                                                                    
[ 62%] Building CXX object src/tracer/CMakeFiles/tracer.dir/stdout_trace_logger.cc.o                                                                  
[ 62%] Building CXX object src/tracer/CMakeFiles/tracer.dir/syslog_trace_logger.cc.o                                                                  
[ 62%] Built target tracer
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/chunk.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/sflsq.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/stats.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/util.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/util_cstring.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/util_jsnorm.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/util_net.cc.o
[ 62%] Building CXX object src/utils/CMakeFiles/utils.dir/util_unfold.cc.o
[ 62%] Built target utils
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/base64_encoder.cc.o                                                                     
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/ber.cc.o
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/boyer_moore.cc.o                                                                        
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/boyer_moore_search.cc.o                                                                 
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/buffer_data.cc.o                                                                        
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/directory.cc.o                                                                          
[ 62%] Building CXX object src/helpers/CMakeFiles/helpers.dir/discovery_filter.cc.o                                                                   
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/json_stream.cc.o                                                                        
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/literal_search.cc.o                                                                     
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/markup.cc.o
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/policy_switcher.cc.o                                                                    
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/sigsafe.cc.o
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/scratch_allocator.cc.o                                                                  
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/streambuf.cc.o                                                                          
[ 63%] Building CXX object src/helpers/CMakeFiles/helpers.dir/utf.cc.o
[ 63%] Built target helpers
[ 63%] Building CXX object src/lua/CMakeFiles/lua.dir/lua.cc.o
[ 63%] Built target lua
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_decomp.cc.o                                                                  
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_decomp_pdf.cc.o                                                              
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_decomp_swf.cc.o                                                              
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_decomp_zip.cc.o                                                              
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_olefile.cc.o                                                                 
[ 63%] Building CXX object src/decompress/CMakeFiles/decompress.dir/file_oleheader.cc.o                                                               
[ 63%] Built target decompress
[ 63%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_detection_filter.cc.o                                                       
[ 63%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_flowbits.cc.o                                                               
[ 63%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_luajit.cc.o                                                                 
[ 63%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_options.cc.o                                                                
[ 63%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_pcre.cc.o                                                                   
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_replace.cc.o                                                                
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_so.cc.o                                                                     
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_vba_data.cc.o                                                               
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ack.cc.o                                                                    
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_base64.cc.o                                                                 
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ber_data.cc.o                                                               
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ber_skip.cc.o                                                               
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_bufferlen.cc.o                                                              
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_byte_extract.cc.o                                                           
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_byte_jump.cc.o                                                              
[ 64%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_byte_math.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_byte_test.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_classtype.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_content.cc.o                                                                
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_cvs.cc.o                                                                    
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_dsize.cc.o                                                                  
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_enable.cc.o                                                                 
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_file_data.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_file_meta.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_file_type.cc.o                                                              
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_flags.cc.o                                                                  
[ 65%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_flow.cc.o                                                                   
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_fragbits.cc.o                                                               
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_fragoffset.cc.o                                                             
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_gid.cc.o                                                                    
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_hash.cc.o                                                                   
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_icmp_id.cc.o                                                                
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_icmp_seq.cc.o                                                               
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_icode.cc.o                                                                  
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_id.cc.o                                                                     
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ipopts.cc.o                                                                 
[ 67%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ip_proto.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_isdataat.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_itype.cc.o                                                                  
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_js_data.cc.o                                                                
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_metadata.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_msg.cc.o                                                                    
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_pkt_data.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_priority.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_raw_data.cc.o                                                               
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_reference.cc.o                                                              
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_rem.cc.o                                                                    
[ 68%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_rev.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_rpc.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_seq.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_service.cc.o                                                                
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_sid.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_soid.cc.o                                                                   
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_tag.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_target.cc.o                                                                 
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_tos.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_ttl.cc.o                                                                    
[ 69%] Building CXX object src/ips_options/CMakeFiles/ips_options.dir/ips_window.cc.o                                                                 
[ 69%] Built target ips_options
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_luajit.cc.o                                                                       
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/log_codecs.cc.o                                                                         
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/loggers.cc.o
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_csv.cc.o                                                                          
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_fast.cc.o                                                                         
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_full.cc.o                                                                         
[ 69%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_json.cc.o                                                                         
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_syslog.cc.o                                                                       
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_talos.cc.o                                                                        
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/alert_unixsock.cc.o                                                                     
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/log_hext.cc.o
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/log_pcap.cc.o
[ 70%] Building CXX object src/loggers/CMakeFiles/loggers.dir/unified2.cc.o
[ 70%] Built target loggers
[ 70%] Building CXX object src/network_inspectors/CMakeFiles/network_inspectors.dir/network_inspectors.cc.o                                           
[ 70%] Built target network_inspectors
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_api.cc.o                                                           
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_app_descriptor.cc.o                                                
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_config.cc.o                                                        
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_cip_event_handler.cc.o                                             
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_data_decrypt_event_handler.cc.o                                    
[ 70%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_debug.cc.o                                                         
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_detector.cc.o                                                      
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_discovery.cc.o                                                     
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_eve_process_event_handler.cc.o                                     
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_ha.cc.o                                                            
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_http_session.cc.o                                                  
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_peg_counts.cc.o                                                    
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_service_event_handler.cc.o                                         
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_session.cc.o                                                       
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_session_api.cc.o                                                   
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_inspector.cc.o                                                     
[ 71%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_module.cc.o                                                        
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_ssh_event_handler.cc.o                                             
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_stats.cc.o                                                         
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/app_info_table.cc.o                                                      
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/host_port_app_cache.cc.o                                                 
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_http_event_handler.cc.o                                            
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/ips_appid_option.cc.o                                                    
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/lua_detector_api.cc.o                                                    
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/lua_detector_flow_api.cc.o                                               
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/lua_detector_module.cc.o                                                 
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_state.cc.o                                                       
[ 72%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/tp_appid_utils.cc.o                                                      
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/tp_lib_handler.cc.o                                                      
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/tp_appid_module_api.cc.o                                                 
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_cpu_profile_table.cc.o                                             
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/user_data_map.cc.o                                                       
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_dns_payload_event_handler.cc.o                                     
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_bit.cc.o                                       
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_bit_tracker.cc.o                               
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_detector.cc.o                                      
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_msn.cc.o                                       
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_rtp.cc.o                                       
[ 73%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_timbuktu.cc.o                                  
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_tns.cc.o                                       
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_app_vnc.cc.o                                       
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/client_discovery.cc.o                                     
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/client_plugins/eve_ca_patterns.cc.o                                      
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/cip_patterns.cc.o                                       
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_dns.cc.o                                       
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_imap.cc.o                                      
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_kerberos.cc.o                                  
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_pattern.cc.o                                   
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_pop3.cc.o                                      
[ 74%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_sip.cc.o                                       
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/detector_smtp.cc.o                                      
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/dns_patterns.cc.o                                       
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/http_url_patterns.cc.o                                  
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/sip_patterns.cc.o                                       
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/ssh_patterns.cc.o                                       
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/detector_plugins/host_patterns.cc.o                                      
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/alpn_patterns.cc.o                                       
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_bgp.cc.o                                         
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_bit.cc.o                                         
[ 75%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_bootp.cc.o                                       
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_dcerpc.cc.o                                      
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_detector.cc.o                                    
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_discovery.cc.o                                   
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_ftp.cc.o                                         
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_irc.cc.o                                         
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_lpr.cc.o                                         
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_mdns.cc.o                                        
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_mysql.cc.o                                       
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_netbios.cc.o                                     
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_nntp.cc.o                                        
[ 76%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_ntp.cc.o                                         
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_radius.cc.o                                      
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_regtest.cc.o                                     
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rexec.cc.o                                       
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rfb.cc.o                                         
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rlogin.cc.o                                      
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rpc.cc.o                                         
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rshell.cc.o                                      
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rsync.cc.o                                       
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_rtmp.cc.o                                        
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_snmp.cc.o                                        
[ 77%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_ssl.cc.o                                         
[ 78%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_telnet.cc.o                                      
[ 78%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_tftp.cc.o                                        
[ 78%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_timbuktu.cc.o                                    
[ 78%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/service_plugins/service_tns.cc.o                                         
[ 78%] Building CXX object src/network_inspectors/appid/CMakeFiles/appid.dir/appid_utils/sf_mlmp.cc.o                                                 
[ 78%] Built target appid
[ 78%] Building CXX object src/network_inspectors/arp_spoof/CMakeFiles/arp_spoof.dir/arp_spoof.cc.o                                                   
[ 78%] Building CXX object src/network_inspectors/arp_spoof/CMakeFiles/arp_spoof.dir/arp_module.cc.o                                                  
[ 78%] Built target arp_spoof
[ 78%] Building CXX object src/network_inspectors/binder/CMakeFiles/binder.dir/binder.cc.o                                                            
[ 78%] Building CXX object src/network_inspectors/binder/CMakeFiles/binder.dir/binding.cc.o                                                           
[ 78%] Building CXX object src/network_inspectors/binder/CMakeFiles/binder.dir/bind_module.cc.o                                                       
[ 78%] Built target binder
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor.cc.o                                                   
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_conn.cc.o                                              
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_csv_logger.cc.o                                        
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_detection.cc.o                                         
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_dns.cc.o                                               
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_file.cc.o                                              
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_flow_data.cc.o                                         
[ 78%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_ftp.cc.o                                               
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_http.cc.o                                              
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_json_logger.cc.o                                       
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_logger.cc.o                                            
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_quic.cc.o                                              
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_service.cc.o                                           
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_ssh.cc.o                                               
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractor_ssl.cc.o                                               
[ 79%] Building CXX object src/network_inspectors/extractor/CMakeFiles/extractor.dir/extractors.cc.o                                                  
[ 79%] Built target extractor
[ 79%] Building CXX object src/network_inspectors/normalize/CMakeFiles/normalize.dir/norm_stats.cc.o                                                  
[ 79%] Building CXX object src/network_inspectors/normalize/CMakeFiles/normalize.dir/normalize.cc.o                                                   
[ 79%] Building CXX object src/network_inspectors/normalize/CMakeFiles/normalize.dir/norm_module.cc.o                                                 
[ 79%] Building CXX object src/network_inspectors/normalize/CMakeFiles/normalize.dir/norm.cc.o                                                        
[ 79%] Built target normalize
[ 79%] Building CXX object src/network_inspectors/packet_capture/CMakeFiles/packet_capture.dir/capture_module.cc.o                                    
[ 79%] Building CXX object src/network_inspectors/packet_capture/CMakeFiles/packet_capture.dir/packet_capture.cc.o                                    
[ 79%] Built target packet_capture
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/base_tracker.cc.o                                          
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/csv_formatter.cc.o                                         
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/cpu_tracker.cc.o                                           
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/flow_tracker.cc.o                                          
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/flow_ip_tracker.cc.o                                       
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/json_formatter.cc.o                                        
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/perf_formatter.cc.o                                        
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/perf_module.cc.o                                           
[ 79%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/perf_monitor.cc.o                                          
[ 80%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/perf_tracker.cc.o                                          
[ 80%] Building CXX object src/network_inspectors/perf_monitor/CMakeFiles/perf_monitor.dir/text_formatter.cc.o                                        
[ 80%] Built target perf_monitor
[ 80%] Building CXX object src/network_inspectors/port_scan/CMakeFiles/port_scan.dir/port_scan.cc.o                                                   
[ 80%] Building CXX object src/network_inspectors/port_scan/CMakeFiles/port_scan.dir/ps_detect.cc.o                                                   
[ 80%] Building CXX object src/network_inspectors/port_scan/CMakeFiles/port_scan.dir/ps_module.cc.o                                                   
[ 80%] Building CXX object src/network_inspectors/port_scan/CMakeFiles/port_scan.dir/ipobj.cc.o                                                       
[ 80%] Built target port_scan
[ 80%] Building CXX object src/network_inspectors/reputation/CMakeFiles/reputation.dir/reputation_commands.cc.o                                       
[ 80%] Building CXX object src/network_inspectors/reputation/CMakeFiles/reputation.dir/reputation_inspect.cc.o                                        
[ 80%] Building CXX object src/network_inspectors/reputation/CMakeFiles/reputation.dir/reputation_module.cc.o                                         
[ 80%] Building CXX object src/network_inspectors/reputation/CMakeFiles/reputation.dir/reputation_parse.cc.o                                          
[ 80%] Built target reputation
[ 80%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/data_purge_cmd.cc.o                                                          
[ 80%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_app_discovery.cc.o                                                       
[ 80%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_event_handler.cc.o                                                       
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint.cc.o                                                         
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint_smb.cc.o                                                     
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint_deviceinfo.cc.o                                              
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint_tcp.cc.o                                                     
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint_ua.cc.o                                                      
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_fingerprint_udp.cc.o                                                     
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_inspector.cc.o                                                           
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_flow.cc.o                                                                
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_logger.cc.o                                                              
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_mac_cache.cc.o                                                           
[ 81%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_module.cc.o                                                              
[ 82%] Building CXX object src/network_inspectors/rna/CMakeFiles/rna.dir/rna_pnd.cc.o                                                                 
[ 82%] Built target rna
[ 82%] Building CXX object src/policy_selectors/CMakeFiles/policy_selectors.dir/policy_selectors.cc.o                                                 
[ 82%] Built target policy_selectors
[ 82%] Building CXX object src/policy_selectors/address_space_selector/CMakeFiles/address_space_selector.dir/address_space_selection.cc.o             
[ 82%] Building CXX object src/policy_selectors/address_space_selector/CMakeFiles/address_space_selector.dir/address_space_selector.cc.o              
[ 82%] Building CXX object src/policy_selectors/address_space_selector/CMakeFiles/address_space_selector.dir/address_space_selector_module.cc.o       
[ 82%] Built target address_space_selector
[ 82%] Building CXX object src/policy_selectors/tenant_selector/CMakeFiles/tenant_selector.dir/tenant_selection.cc.o                                  
[ 82%] Building CXX object src/policy_selectors/tenant_selector/CMakeFiles/tenant_selector.dir/tenant_selector.cc.o                                   
[ 82%] Building CXX object src/policy_selectors/tenant_selector/CMakeFiles/tenant_selector.dir/tenant_selector_module.cc.o                            
[ 82%] Built target tenant_selector
[ 82%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/search_engines.cc.o                                                       
[ 82%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/search_tool.cc.o                                                          
[ 82%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/ac_bnfa.cc.o                                                              
[ 82%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/bnfa_search.cc.o                                                          
[ 83%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/ac_full.cc.o                                                              
[ 83%] Building CXX object src/search_engines/CMakeFiles/search_engines.dir/acsmx2.cc.o                                                               
[ 83%] Built target search_engines
[ 84%] Building CXX object src/side_channel/CMakeFiles/side_channel.dir/side_channel.cc.o                                                             
[ 84%] Building CXX object src/side_channel/CMakeFiles/side_channel.dir/side_channel_module.cc.o                                                      
[ 84%] Building CXX object src/side_channel/CMakeFiles/side_channel.dir/side_channel_format.cc.o                                                      
[ 84%] Built target side_channel
[ 84%] Building CXX object src/connectors/CMakeFiles/connectors.dir/connectors.cc.o                                                                   
[ 84%] Built target connectors
[ 84%] Building CXX object src/connectors/file_connector/CMakeFiles/file_connector.dir/file_connector.cc.o                                            
[ 84%] Building CXX object src/connectors/file_connector/CMakeFiles/file_connector.dir/file_connector_module.cc.o                                     
[ 84%] Built target file_connector
[ 84%] Building CXX object src/connectors/tcp_connector/CMakeFiles/tcp_connector.dir/tcp_connector.cc.o                                               
[ 84%] Building CXX object src/connectors/tcp_connector/CMakeFiles/tcp_connector.dir/tcp_connector_module.cc.o                                        
[ 84%] Built target tcp_connector
[ 84%] Building CXX object src/connectors/std_connector/CMakeFiles/std_connector.dir/std_connector_buffer.cc.o                                        
[ 84%] Building CXX object src/connectors/std_connector/CMakeFiles/std_connector.dir/std_connector.cc.o                                               
[ 84%] Built target std_connector
[ 85%] Building CXX object src/mp_transport/CMakeFiles/mp_transports.dir/mp_transports.cc.o                                                           
[ 85%] Built target mp_transports
[ 85%] Building CXX object src/CMakeFiles/snort.dir/main.cc.o
[ 85%] Linking CXX executable snort
[ 85%] Built target snort
[ 85%] Generating api_options.h
[ 85%] Built target api_options
[ 85%] Generating snort_api.h
[ 85%] Built target snort_api
[ 85%] Building CXX object tools/u2boat/CMakeFiles/u2boat.dir/u2boat.cc.o
[ 85%] Linking CXX executable u2boat
[ 85%] Built target u2boat
[ 85%] Building CXX object tools/u2spewfoo/CMakeFiles/u2spewfoo.dir/u2spewfoo.cc.o                                                                    
[ 85%] Linking CXX executable u2spewfoo
[ 85%] Built target u2spewfoo
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_base64_decode.cc.o                                             
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_content.cc.o                                                   
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_convert_comma_list.cc.o                                        
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_dce_iface.cc.o                                                 
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_dnp3_obj.cc.o                                                  
[ 85%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_dsize.cc.o                                                     
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_file_data.cc.o                                                 
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_file_type.cc.o                                                 
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_gid_sid.cc.o                                                   
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_http_encode.cc.o                                               
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_isdataat.cc.o                                                  
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_metadata.cc.o                                                  
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_pcre.cc.o                                                      
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_react.cc.o                                                     
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_reference.cc.o                                                 
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_replace.cc.o                                                   
[ 86%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_resp.cc.o                                                      
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_sd_pattern.cc.o                                                
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_stream_reassemble.cc.o                                         
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_stream_size.cc.o                                               
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_tag.cc.o                                                       
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_threshold.cc.o                                                 
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_ttl.cc.o                                                       
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_unchanged.cc.o                                                 
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_unsupported.cc.o                                               
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_urilen.cc.o                                                    
[ 87%] Building CXX object tools/snort2lua/rule_states/CMakeFiles/rule_states.dir/rule_api.cc.o                                                       
[ 87%] Built target rule_states
[ 87%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_alertfile.cc.o                                           
[ 87%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_binding.cc.o                                             
[ 87%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_checksums.cc.o                                           
[ 87%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_classification.cc.o                                      
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_daq.cc.o                                                 
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_daq_mode.cc.o                                            
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_daq_var.cc.o                                             
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_decode_esp.cc.o                                          
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_default_rule_state.cc.o                                  
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_deleted.cc.o                                             
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_detection.cc.o                                           
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_event_trace.cc.o                                         
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_file.cc.o                                                
[ 88%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_event_queue.cc.o                                         
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_ignore_ports.cc.o                                        
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_ipv6_frag.cc.o                                           
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_memcaps.cc.o                                             
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_mpls_payload_type.cc.o                                   
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_na_policy_mode.cc.o                                      
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_no_option.cc.o                                           
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_one_int_option.cc.o                                      
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_one_string_option.cc.o                                   
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_order.cc.o                                               
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_paf_max.cc.o                                             
[ 89%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_policy_id.cc.o                                           
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_policy_mode.cc.o                                         
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_policy_uuid.cc.o                                         
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_ppm.cc.o                                                 
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_profile.cc.o                                             
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_reference.cc.o                                           
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_response.cc.o                                            
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_tunnel_verdicts.cc.o                                     
[ 90%] Building CXX object tools/snort2lua/config_states/CMakeFiles/config_states.dir/config_api.cc.o                                                 
[ 90%] Built target config_states
[ 90%] Building CXX object tools/snort2lua/data/CMakeFiles/conversion_data.dir/dt_data.cc.o                                                           
[ 91%] Building CXX object tools/snort2lua/data/CMakeFiles/conversion_data.dir/dt_rule_api.cc.o                                                       
[ 91%] Building CXX object tools/snort2lua/data/CMakeFiles/conversion_data.dir/dt_state_api.cc.o                                                      
[ 91%] Building CXX object tools/snort2lua/data/CMakeFiles/conversion_data.dir/dt_table_api.cc.o                                                      
[ 91%] Built target conversion_data
[ 91%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_comment.cc.o                                                  
[ 91%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_include.cc.o                                                  
[ 91%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_option.cc.o                                                   
[ 91%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_table.cc.o                                                    
[ 92%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_rule.cc.o                                                     
[ 92%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_rule_option.cc.o                                              
[ 92%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_rule_suboption.cc.o                                           
[ 92%] Building CXX object tools/snort2lua/data/data_types/CMakeFiles/data_types.dir/dt_var.cc.o                                                      
[ 92%] Built target data_types
[ 92%] Building CXX object tools/snort2lua/helpers/CMakeFiles/snort2lua_helpers.dir/converter.cc.o                                                    
[ 92%] Building CXX object tools/snort2lua/helpers/CMakeFiles/snort2lua_helpers.dir/s2l_util.cc.o                                                     
[ 92%] Building CXX object tools/snort2lua/helpers/CMakeFiles/snort2lua_helpers.dir/parse_cmd_line.cc.o                                               
[ 92%] Building CXX object tools/snort2lua/helpers/CMakeFiles/snort2lua_helpers.dir/util_binder.cc.o                                                  
[ 92%] Building CXX object tools/snort2lua/helpers/CMakeFiles/snort2lua_helpers.dir/s2l_markup.cc.o                                                   
[ 92%] Built target snort2lua_helpers
[ 92%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_attribute_table.cc.o                                      
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_config.cc.o                                               
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_deleted.cc.o                                              
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_event_filter.cc.o                                         
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_file.cc.o                                                 
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_include.cc.o                                              
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_output.cc.o                                               
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_paths.cc.o                                                
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_preprocessor.cc.o                                         
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_rate_filter.cc.o                                          
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_rule.cc.o                                                 
[ 93%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_rule_state.cc.o                                           
[ 94%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_ruletype.cc.o                                             
[ 94%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_var.cc.o                                                  
[ 94%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/kws_suppress.cc.o                                             
[ 94%] Building CXX object tools/snort2lua/keyword_states/CMakeFiles/keyword_states.dir/keywords_api.cc.o                                             
[ 94%] Built target keyword_states
[ 94%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_csv.cc.o                                                    
[ 94%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_deleted.cc.o                                                
[ 94%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_fast.cc.o                                                   
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_full.cc.o                                                   
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_null.cc.o                                                   
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_tcpdump.cc.o                                                
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_test.cc.o                                                   
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_syslog.cc.o                                                 
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_unified2.cc.o                                               
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/out_unixsock.cc.o                                               
[ 95%] Building CXX object tools/snort2lua/output_states/CMakeFiles/output_states.dir/output_api.cc.o                                                 
[ 95%] Built target output_states
[ 95%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_appid.cc.o                                      
[ 95%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_arpspoof.cc.o                                   
[ 95%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_bo.cc.o                                         
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_dcerpc.cc.o                                     
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_dcerpc_server.cc.o                              
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_dnp3.cc.o                                       
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_frag3_engine.cc.o                               
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_frag3_global.cc.o                               
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_ftp_telnet.cc.o                                 
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_ftp_telnet_protocol.cc.o                        
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_gtp.cc.o                                        
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_http_inspect.cc.o                               
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_http_inspect_server.cc.o                        
[ 96%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_normalizers.cc.o                                
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_perfmonitor.cc.o                                
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_reputation.cc.o                                 
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_rpc_decode.cc.o                                 
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_sdf.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_sip.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_ssh.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_ssl.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_dns.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_pop.cc.o                                        
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_imap.cc.o                                       
[ 97%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_modbus.cc.o                                     
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_rna.cc.o                                        
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_smtp.cc.o                                       
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_sfportscan.cc.o                                 
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_stream5_ip.cc.o                                 
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_stream5_global.cc.o                             
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_stream5_tcp.cc.o                                
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_stream5_udp.cc.o                                
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/pps_stream5_ha.cc.o                                 
[ 98%] Building CXX object tools/snort2lua/preprocessor_states/CMakeFiles/preprocessor_states.dir/preprocessor_api.cc.o                               
[ 98%] Built target preprocessor_states
[ 98%] Building CXX object tools/snort2lua/CMakeFiles/snort2lua.dir/snort2lua.cc.o                                                                    
[100%] Building CXX object tools/snort2lua/CMakeFiles/snort2lua.dir/init_state.cc.o                                                                   
[100%] Linking CXX executable snort2lua
[100%] Built target snort2lua
[100%] Building CXX object tools/show_flows/CMakeFiles/show_flows.dir/show_flows.cc.o                                                                 
[100%] Linking CXX executable show_flows
[100%] Built target show_flows
[100%] Building C object daqs/CMakeFiles/daq_file.dir/daq_file.c.o
[100%] Linking C shared module daq_file.so
[100%] Built target daq_file
[100%] Building C object daqs/CMakeFiles/daq_hext.dir/daq_hext.c.o
[100%] Linking C shared module daq_hext.so
[100%] Built target daq_hext
                                                                           
┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo make install
[sudo] password for kali: 
[  0%] Built target unixdomain_connector
[  2%] Built target framework
[  2%] Built target mp_unix_transport
[  3%] Built target ips_actions
[  3%] Built target codecs
[  3%] Built target root_codecs
[  4%] Built target link_codecs
[  6%] Built target ip_codecs
[  7%] Built target misc_codecs
[  7%] Built target control
[ 10%] Built target detection
[ 10%] Built target dump_config
[ 11%] Built target events
[ 13%] Built target file_api
[ 13%] Built target filter
[ 14%] Built target flow
[ 15%] Built target hash
[ 16%] Built target js_norm
[ 16%] Built target latency
[ 17%] Built target log
[ 19%] Built target main
[ 20%] Built target managers
[ 21%] Built target memory
[ 22%] Built target mime
[ 23%] Built target packet_io
[ 24%] Built target parser
[ 25%] Built target payload_injector
[ 26%] Built target ports
[ 27%] Built target protocols
[ 27%] Built target sfip
[ 27%] Built target sfrt
[ 27%] Built target service_inspectors
[ 27%] Built target back_orifice
[ 29%] Built target cip
[ 32%] Built target dce_rpc
[ 32%] Built target dnp3
[ 34%] Built target dns
[ 35%] Built target ftp_telnet
[ 36%] Built target gtp_inspect
[ 40%] Built target http_inspect
[ 42%] Built target http2_inspect
[ 43%] Built target iec104
[ 43%] Built target imap
[ 44%] Built target mms
[ 44%] Built target modbus
[ 44%] Built target netflow
[ 45%] Built target opcua
[ 45%] Built target pop
[ 45%] Built target rpc_decode
[ 46%] Built target s7commplus
[ 47%] Built target sip
[ 47%] Built target smtp
[ 47%] Built target ssh
[ 48%] Built target ssl
[ 48%] Built target tlv_pdu
[ 50%] Built target wizard
[ 51%] Built target socks
[ 51%] Built target stream
[ 52%] Built target stream_paf
[ 52%] Built target stream_base
[ 52%] Built target stream_ip
[ 52%] Built target stream_icmp
[ 55%] Built target stream_tcp
[ 56%] Built target stream_udp
[ 56%] Built target stream_user
[ 57%] Built target stream_file
[ 57%] Built target target_based
[ 58%] Built target host_tracker
[ 59%] Built target pub_sub
[ 60%] Built target time
[ 61%] Built target profiler
[ 61%] Built target trace
[ 62%] Built target tracer
[ 62%] Built target utils
[ 63%] Built target helpers
[ 63%] Built target lua
[ 63%] Built target decompress
[ 69%] Built target ips_options
[ 70%] Built target loggers
[ 70%] Built target network_inspectors
[ 78%] Built target appid
[ 78%] Built target arp_spoof
[ 78%] Built target binder
[ 79%] Built target extractor
[ 79%] Built target normalize
[ 79%] Built target packet_capture
[ 80%] Built target perf_monitor
[ 80%] Built target port_scan
[ 80%] Built target reputation
[ 82%] Built target rna
[ 82%] Built target policy_selectors
[ 82%] Built target address_space_selector
[ 82%] Built target tenant_selector
[ 83%] Built target search_engines
[ 84%] Built target side_channel
[ 84%] Built target connectors
[ 84%] Built target file_connector
[ 84%] Built target tcp_connector
[ 84%] Built target std_connector
[ 85%] Built target mp_transports
[ 85%] Built target snort
[ 85%] Built target api_options
[ 85%] Built target snort_api
[ 85%] Built target u2boat
[ 85%] Built target u2spewfoo
[ 87%] Built target rule_states
[ 90%] Built target config_states
[ 91%] Built target conversion_data
[ 92%] Built target data_types
[ 92%] Built target snort2lua_helpers
[ 94%] Built target keyword_states
[ 95%] Built target output_states
[ 98%] Built target preprocessor_states
[100%] Built target snort2lua
[100%] Built target show_flows
[100%] Built target daq_file
[100%] Built target daq_hext
Install the project...
-- Install configuration: ""
-- Installing: /usr/local/lib/pkgconfig/snort.pc
-- Installing: /usr/local/bin/snort
-- Installing: /usr/local/include/snort/codecs/codec_module.h
-- Installing: /usr/local/include/snort/control/control.h
-- Installing: /usr/local/include/snort/detection/detection_buf.h
-- Installing: /usr/local/include/snort/detection/detection_engine.h
-- Installing: /usr/local/include/snort/detection/extract.h
-- Installing: /usr/local/include/snort/detection/ips_context.h
-- Installing: /usr/local/include/snort/detection/ips_context_chain.h
-- Installing: /usr/local/include/snort/detection/ips_context_data.h
-- Installing: /usr/local/include/snort/detection/pattern_match_data.h
-- Installing: /usr/local/include/snort/detection/rule_option_types.h
-- Installing: /usr/local/include/snort/events/event.h
-- Installing: /usr/local/include/snort/file_api/file_api.h
-- Installing: /usr/local/include/snort/file_api/file_capture.h
-- Installing: /usr/local/include/snort/file_api/file_flows.h
-- Installing: /usr/local/include/snort/file_api/file_lib.h
-- Installing: /usr/local/include/snort/file_api/file_service.h
-- Installing: /usr/local/include/snort/flow/deferred_trust.h
-- Installing: /usr/local/include/snort/flow/dump_flows.h
-- Installing: /usr/local/include/snort/flow/dump_flows_descriptor.h
-- Installing: /usr/local/include/snort/flow/dump_flows_serializer.h
-- Installing: /usr/local/include/snort/flow/expect_flow.h
-- Installing: /usr/local/include/snort/flow/flow.h
-- Installing: /usr/local/include/snort/flow/flow_data.h
-- Installing: /usr/local/include/snort/flow/flow_key.h
-- Installing: /usr/local/include/snort/flow/flow_stash.h
-- Installing: /usr/local/include/snort/flow/ha.h
-- Installing: /usr/local/include/snort/flow/prune_stats.h
-- Installing: /usr/local/include/snort/flow/session.h
-- Installing: /usr/local/include/snort/flow/stream_flow.h
-- Installing: /usr/local/include/snort/framework/base_api.h
-- Installing: /usr/local/include/snort/framework/codec.h
-- Installing: /usr/local/include/snort/framework/connector.h
-- Installing: /usr/local/include/snort/framework/counts.h
-- Installing: /usr/local/include/snort/framework/cursor.h
-- Installing: /usr/local/include/snort/framework/data_bus.h
-- Installing: /usr/local/include/snort/framework/decode_data.h
-- Installing: /usr/local/include/snort/framework/endianness.h
-- Installing: /usr/local/include/snort/framework/inspector.h
-- Installing: /usr/local/include/snort/framework/ips_action.h
-- Installing: /usr/local/include/snort/framework/ips_option.h
-- Installing: /usr/local/include/snort/framework/logger.h
-- Installing: /usr/local/include/snort/framework/module.h
-- Installing: /usr/local/include/snort/framework/mp_data_bus.h
-- Installing: /usr/local/include/snort/framework/mp_transport.h
-- Installing: /usr/local/include/snort/framework/mpse_batch.h
-- Installing: /usr/local/include/snort/framework/mpse.h
-- Installing: /usr/local/include/snort/framework/parameter.h
-- Installing: /usr/local/include/snort/framework/pdu_section.h
-- Installing: /usr/local/include/snort/framework/pig_pen.h
-- Installing: /usr/local/include/snort/framework/plugins.h
-- Installing: /usr/local/include/snort/framework/policy_selector.h
-- Installing: /usr/local/include/snort/framework/range.h
-- Installing: /usr/local/include/snort/framework/so_rule.h
-- Installing: /usr/local/include/snort/framework/tracer.h
-- Installing: /usr/local/include/snort/framework/value.h
-- Installing: /usr/local/include/snort/framework/api_options.h
-- Installing: /usr/local/include/snort/framework/snort_api.h
-- Installing: /usr/local/include/snort/hash/hashes.h
-- Installing: /usr/local/include/snort/hash/hash_key_operations.h
-- Installing: /usr/local/include/snort/hash/lru_cache_local.h
-- Installing: /usr/local/include/snort/hash/lru_cache_shared.h
-- Installing: /usr/local/include/snort/hash/lru_segmented_cache_shared.h
-- Installing: /usr/local/include/snort/hash/xhash.h
-- Installing: /usr/local/include/snort/log/log_stats.h
-- Installing: /usr/local/include/snort/log/log_text.h
-- Installing: /usr/local/include/snort/log/messages.h
-- Installing: /usr/local/include/snort/log/obfuscator.h
-- Installing: /usr/local/include/snort/log/text_log.h
-- Installing: /usr/local/include/snort/log/unified2.h
-- Installing: /usr/local/include/snort/log/u2_packet.h
-- Installing: /usr/local/include/snort/main/analyzer_command.h
-- Installing: /usr/local/include/snort/main/policy.h
-- Installing: /usr/local/include/snort/main/reload_tracker.h
-- Installing: /usr/local/include/snort/main/reload_tuner.h
-- Installing: /usr/local/include/snort/main/snort_config.h
-- Installing: /usr/local/include/snort/main/snort_types.h
-- Installing: /usr/local/include/snort/main/thread.h
-- Installing: /usr/local/include/snort/main/thread_config.h
-- Installing: /usr/local/include/snort/main/snort.h
-- Installing: /usr/local/include/snort/lua/snort_plugin.lua
-- Installing: /usr/local/include/snort/memory/heap_interface.h
-- Installing: /usr/local/include/snort/memory/memory_cap.h
-- Installing: /usr/local/include/snort/mime/decode_b64.h
-- Installing: /usr/local/include/snort/mime/decode_base.h
-- Installing: /usr/local/include/snort/mime/file_mime_config.h
-- Installing: /usr/local/include/snort/mime/file_mime_decode.h
-- Installing: /usr/local/include/snort/mime/file_mime_form_data.h
-- Installing: /usr/local/include/snort/mime/file_mime_log.h
-- Installing: /usr/local/include/snort/mime/file_mime_paf.h
-- Installing: /usr/local/include/snort/mime/file_mime_process.h
-- Installing: /usr/local/include/snort/packet_io/active.h
-- Installing: /usr/local/include/snort/packet_io/active_action.h
-- Installing: /usr/local/include/snort/packet_io/packet_constraints.h
-- Installing: /usr/local/include/snort/packet_io/packet_tracer.h
-- Installing: /usr/local/include/snort/packet_io/sfdaq.h
-- Installing: /usr/local/include/snort/packet_io/sfdaq_instance.h
-- Installing: /usr/local/include/snort/payload_injector/payload_injector.h
-- Installing: /usr/local/include/snort/protocols/arp.h
-- Installing: /usr/local/include/snort/protocols/bpdu.h
-- Installing: /usr/local/include/snort/protocols/cdp.h
-- Installing: /usr/local/include/snort/protocols/cisco_meta_data.h
-- Installing: /usr/local/include/snort/protocols/eapol.h
-- Installing: /usr/local/include/snort/protocols/eth.h
-- Installing: /usr/local/include/snort/protocols/icmp4.h
-- Installing: /usr/local/include/snort/protocols/icmp6.h
-- Installing: /usr/local/include/snort/protocols/ip.h
-- Installing: /usr/local/include/snort/protocols/ipv4.h
-- Installing: /usr/local/include/snort/protocols/ipv4_options.h
-- Installing: /usr/local/include/snort/protocols/ipv6.h
-- Installing: /usr/local/include/snort/protocols/geneve.h
-- Installing: /usr/local/include/snort/protocols/gre.h
-- Installing: /usr/local/include/snort/protocols/layer.h
-- Installing: /usr/local/include/snort/protocols/linux_sll.h
-- Installing: /usr/local/include/snort/protocols/mpls.h
-- Installing: /usr/local/include/snort/protocols/packet.h
-- Installing: /usr/local/include/snort/protocols/packet_manager.h
-- Installing: /usr/local/include/snort/protocols/protocol_ids.h
-- Installing: /usr/local/include/snort/protocols/ssl.h
-- Installing: /usr/local/include/snort/protocols/tcp.h
-- Installing: /usr/local/include/snort/protocols/tcp_options.h
-- Installing: /usr/local/include/snort/protocols/teredo.h
-- Installing: /usr/local/include/snort/protocols/token_ring.h
-- Installing: /usr/local/include/snort/protocols/udp.h
-- Installing: /usr/local/include/snort/protocols/wlan.h
-- Installing: /usr/local/include/snort/protocols/vlan.h
-- Installing: /usr/local/include/snort/sfip/sf_cidr.h
-- Installing: /usr/local/include/snort/sfip/sf_ip.h
-- Installing: /usr/local/include/snort/sfip/sf_returns.h
-- Installing: /usr/local/include/snort/service_inspectors/ftp_telnet/ftp_data.h
-- Installing: /usr/local/include/snort/service_inspectors/ftp_telnet/ftpdata_splitter.h
-- Installing: /usr/local/include/snort/service_inspectors/ftp_telnet/ftp_module.h
-- Installing: /usr/local/include/snort/service_inspectors/ftp_telnet/ftpp_ui_config.h
-- Installing: /usr/local/include/snort/service_inspectors/ftp_telnet/kmap.h
-- Installing: /usr/local/include/snort/service_inspectors/http_inspect/http_field.h
-- Installing: /usr/local/include/snort/service_inspectors/http_inspect/http_common.h
-- Installing: /usr/local/include/snort/service_inspectors/http_inspect/http_inspect_base.h
-- Installing: /usr/local/include/snort/service_inspectors/http_inspect/http_stream_splitter_base.h
-- Installing: /usr/local/include/snort/service_inspectors/http_inspect/http_test_manager.h
-- Installing: /usr/local/include/snort/service_inspectors/http2_inspect/http2_huffman_state_machine.h
-- Installing: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_int_decode.h
-- Installing: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_int_decode_impl.h
-- Installing: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_string_decode.h
-- Installing: /usr/local/include/snort/service_inspectors/http2_inspect/http2_varlen_string_decode_impl.h
-- Installing: /usr/local/include/snort/service_inspectors/netflow/netflow_record.h
-- Installing: /usr/local/include/snort/service_inspectors/ssh/ssh_types.h
-- Installing: /usr/local/include/snort/service_inspectors/ssl/ssl_flow_data.h
-- Installing: /usr/local/include/snort/stream/flush_bucket.h
-- Installing: /usr/local/include/snort/stream/paf.h
-- Installing: /usr/local/include/snort/stream/pafng.h
-- Installing: /usr/local/include/snort/stream/stream.h
-- Installing: /usr/local/include/snort/stream/stream_splitter.h
-- Installing: /usr/local/include/snort/stream/udp/udp_session.h
-- Installing: /usr/local/include/snort/target_based/snort_protocols.h
-- Installing: /usr/local/include/snort/host_tracker/cache_allocator.h
-- Installing: /usr/local/include/snort/host_tracker/cache_interface.h
-- Installing: /usr/local/include/snort/host_tracker/host_cache.h
-- Installing: /usr/local/include/snort/host_tracker/host_tracker.h
-- Installing: /usr/local/include/snort/pub_sub/appid_debug_log_event.h
-- Installing: /usr/local/include/snort/pub_sub/appid_event_ids.h
-- Installing: /usr/local/include/snort/pub_sub/appid_events.h
-- Installing: /usr/local/include/snort/pub_sub/assistant_gadget_event.h
-- Installing: /usr/local/include/snort/pub_sub/cip_events.h
-- Installing: /usr/local/include/snort/pub_sub/daq_message_event.h
-- Installing: /usr/local/include/snort/pub_sub/data_decrypt_event.h
-- Installing: /usr/local/include/snort/pub_sub/dcerpc_events.h
-- Installing: /usr/local/include/snort/pub_sub/detection_events.h
-- Installing: /usr/local/include/snort/pub_sub/dhcp_events.h
-- Installing: /usr/local/include/snort/pub_sub/dns_events.h
-- Installing: /usr/local/include/snort/pub_sub/domain_fronting.h
-- Installing: /usr/local/include/snort/pub_sub/eof_event.h
-- Installing: /usr/local/include/snort/pub_sub/eve_process_event.h
-- Installing: /usr/local/include/snort/pub_sub/expect_events.h
-- Installing: /usr/local/include/snort/pub_sub/external_event_ids.h
-- Installing: /usr/local/include/snort/pub_sub/file_events_ids.h
-- Installing: /usr/local/include/snort/pub_sub/file_events.h
-- Installing: /usr/local/include/snort/pub_sub/finalize_packet_event.h
-- Installing: /usr/local/include/snort/pub_sub/ftp_events.h
-- Installing: /usr/local/include/snort/pub_sub/http_body_event.h
-- Installing: /usr/local/include/snort/pub_sub/http_event_ids.h
-- Installing: /usr/local/include/snort/pub_sub/http_events.h
-- Installing: /usr/local/include/snort/pub_sub/http_form_data_event.h
-- Installing: /usr/local/include/snort/pub_sub/http_publish_length_event.h
-- Installing: /usr/local/include/snort/pub_sub/http_request_body_event.h
-- Installing: /usr/local/include/snort/pub_sub/http_transaction_end_event.h
-- Installing: /usr/local/include/snort/pub_sub/intrinsic_event_ids.h
-- Installing: /usr/local/include/snort/pub_sub/netflow_event.h
-- Installing: /usr/local/include/snort/pub_sub/opportunistic_tls_event.h
-- Installing: /usr/local/include/snort/pub_sub/packet_events.h
-- Installing: /usr/local/include/snort/pub_sub/quic_events.h
-- Installing: /usr/local/include/snort/pub_sub/reputation_events.h
-- Installing: /usr/local/include/snort/pub_sub/rna_events.h
-- Installing: /usr/local/include/snort/pub_sub/shadowtraffic_aggregator.h
-- Installing: /usr/local/include/snort/pub_sub/sip_events.h
-- Installing: /usr/local/include/snort/pub_sub/smb_events.h
-- Installing: /usr/local/include/snort/pub_sub/ssh_events.h
-- Installing: /usr/local/include/snort/pub_sub/ssl_events.h
-- Installing: /usr/local/include/snort/pub_sub/stream_event_ids.h
-- Installing: /usr/local/include/snort/pub_sub/dns_payload_event.h
-- Installing: /usr/local/include/snort/pub_sub/deviceinfo_events.h
-- Installing: /usr/local/include/snort/time/clock_defs.h
-- Installing: /usr/local/include/snort/time/packet_time.h
-- Installing: /usr/local/include/snort/time/periodic.h
-- Installing: /usr/local/include/snort/time/stopwatch.h
-- Installing: /usr/local/include/snort/profiler/memory_defs.h
-- Installing: /usr/local/include/snort/profiler/memory_profiler_defs.h
-- Installing: /usr/local/include/snort/profiler/profiler.h
-- Installing: /usr/local/include/snort/profiler/profiler_defs.h
-- Installing: /usr/local/include/snort/profiler/rule_profiler_defs.h
-- Installing: /usr/local/include/snort/profiler/time_profiler_defs.h
-- Installing: /usr/local/include/snort/trace/trace.h
-- Installing: /usr/local/include/snort/trace/trace_api.h
-- Installing: /usr/local/include/snort/utils/bits.h
-- Installing: /usr/local/include/snort/utils/cpp_macros.h
-- Installing: /usr/local/include/snort/utils/endian.h
-- Installing: /usr/local/include/snort/utils/safec.h
-- Installing: /usr/local/include/snort/utils/util.h
-- Installing: /usr/local/include/snort/utils/util_cstring.h
-- Installing: /usr/local/include/snort/utils/util_unfold.h
-- Installing: /usr/local/include/snort/helpers/base64_encoder.h
-- Installing: /usr/local/include/snort/helpers/ber.h
-- Installing: /usr/local/include/snort/helpers/bitop.h
-- Installing: /usr/local/include/snort/helpers/boyer_moore.h
-- Installing: /usr/local/include/snort/helpers/boyer_moore_search.h
-- Installing: /usr/local/include/snort/helpers/buffer_data.h
-- Installing: /usr/local/include/snort/helpers/event_gen.h
-- Installing: /usr/local/include/snort/helpers/infractions.h
-- Installing: /usr/local/include/snort/helpers/json_stream.h
-- Installing: /usr/local/include/snort/helpers/literal_search.h
-- Installing: /usr/local/include/snort/helpers/lockless_ring.h
-- Installing: /usr/local/include/snort/helpers/memcap_allocator.h
-- Installing: /usr/local/include/snort/helpers/ring2.h
-- Installing: /usr/local/include/snort/helpers/scratch_allocator.h
-- Installing: /usr/local/include/snort/helpers/sigsafe.h
-- Installing: /usr/local/include/snort/helpers/utf.h
-- Installing: /usr/local/include/snort/decompress/file_decomp.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_api.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_app_descriptor.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_debug.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_dns_session.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_http_session.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_session_api.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/appid_types.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/application_ids.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/tp_appid_module_api.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/tp_appid_session_api.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/tp_appid_types.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/mp_data_bus.h
-- Installing: /usr/local/include/snort/network_inspectors/appid/mp_data_bus.cc
-- Installing: /usr/local/include/snort/network_inspectors/extractor/extractor_enums.h
-- Installing: /usr/local/include/snort/network_inspectors/reputation/reputation_common.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_cpe_os.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_deviceinfo.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_smb.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_tcp.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_ua.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_fingerprint_udp.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_inspector.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_logger_event.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_name.h
-- Installing: /usr/local/include/snort/network_inspectors/rna/rna_tracker.h
-- Installing: /usr/local/include/snort/search_engines/search_common.h
-- Installing: /usr/local/include/snort/search_engines/search_tool.h
-- Installing: /usr/local/bin/appid_detector_builder.sh
-- Installing: /usr/local/bin/u2boat
-- Installing: /usr/local/share/doc/snort/README.u2boat
-- Installing: /usr/local/bin/u2spewfoo
-- Installing: /usr/local/bin/snort2lua
-- Installing: /usr/local/bin/show_flows
-- Installing: /usr/local/share/doc/snort/README.show_flows
-- Installing: /usr/local/etc/snort/balanced.lua
-- Installing: /usr/local/etc/snort/connectivity.lua
-- Installing: /usr/local/etc/snort/file_magic.rules
-- Installing: /usr/local/etc/snort/inline.lua
-- Installing: /usr/local/etc/snort/max_detect.lua
-- Installing: /usr/local/etc/snort/sensitive_data.rules
-- Installing: /usr/local/etc/snort/security.lua
-- Installing: /usr/local/etc/snort/snort.lua
-- Installing: /usr/local/etc/snort/snort_defaults.lua
-- Installing: /usr/local/etc/snort/talos.lua
-- Installing: /usr/local/lib/snort/daq/daq_file.so
-- Installing: /usr/local/lib/snort/daq/daq_hext.so
-- Installing: /usr/local/include/snort/daq/daq_user.h
-- Installing: /usr/local/share/doc/snort/active.txt
-- Installing: /usr/local/share/doc/snort/appid.txt
-- Installing: /usr/local/share/doc/snort/binder.txt
-- Installing: /usr/local/share/doc/snort/byte_extract.txt
-- Installing: /usr/local/share/doc/snort/byte_jump.txt
-- Installing: /usr/local/share/doc/snort/byte_math.txt
-- Installing: /usr/local/share/doc/snort/byte_options.txt
-- Installing: /usr/local/share/doc/snort/byte_test.txt
-- Installing: /usr/local/share/doc/snort/concepts.txt
-- Installing: /usr/local/share/doc/snort/connectors.txt
-- Installing: /usr/local/share/doc/snort/dump_config.txt
-- Installing: /usr/local/share/doc/snort/daq.txt
-- Installing: /usr/local/share/doc/snort/dcerpc.txt
-- Installing: /usr/local/share/doc/snort/errors.txt
-- Installing: /usr/local/share/doc/snort/extractor.txt
-- Installing: /usr/local/share/doc/snort/features.txt
-- Installing: /usr/local/share/doc/snort/file_processing.txt
-- Installing: /usr/local/share/doc/snort/ftp.txt
-- Installing: /usr/local/share/doc/snort/high_availability.txt
-- Installing: /usr/local/share/doc/snort/http_inspect.txt
-- Installing: /usr/local/share/doc/snort/http2_inspect.txt
-- Installing: /usr/local/share/doc/snort/iec104.txt
-- Installing: /usr/local/share/doc/snort/js_norm.txt
-- Installing: /usr/local/share/doc/snort/mms.txt
-- Installing: /usr/local/share/doc/snort/opcua.txt
-- Installing: /usr/local/share/doc/snort/overview.txt
-- Installing: /usr/local/share/doc/snort/params.txt
-- Installing: /usr/local/share/doc/snort/perf_monitor.txt
-- Installing: /usr/local/share/doc/snort/pop_imap.txt
-- Installing: /usr/local/share/doc/snort/port_scan.txt
-- Installing: /usr/local/share/doc/snort/sensitive_data.txt
-- Installing: /usr/local/share/doc/snort/side_channel.txt
-- Installing: /usr/local/share/doc/snort/smtp.txt
-- Installing: /usr/local/share/doc/snort/snort2x.png
-- Installing: /usr/local/share/doc/snort/snort3x.png
-- Installing: /usr/local/share/doc/snort/snort_user.txt
-- Installing: /usr/local/share/doc/snort/snorty.png
-- Installing: /usr/local/share/doc/snort/telnet.txt
-- Installing: /usr/local/share/doc/snort/terms.txt
-- Installing: /usr/local/share/doc/snort/trace.txt
-- Installing: /usr/local/share/doc/snort/tutorial.txt
-- Installing: /usr/local/share/doc/snort/usage.txt
-- Installing: /usr/local/share/doc/snort/wizard.txt
-- Installing: /usr/local/share/doc/snort/snort_user.text
-- Installing: /usr/local/share/doc/snort/appendix.txt
-- Installing: /usr/local/share/doc/snort/building.txt
-- Installing: /usr/local/share/doc/snort/builtin_stubs.txt
-- Installing: /usr/local/share/doc/snort/enviro.txt
-- Installing: /usr/local/share/doc/snort/snort_reference.txt
-- Installing: /usr/local/share/doc/snort/snort_reference.text
-- Installing: /usr/local/share/doc/snort/differences.txt
-- Up-to-date: /usr/local/share/doc/snort/overview.txt
-- Installing: /usr/local/share/doc/snort/snort2lua.txt
-- Installing: /usr/local/share/doc/snort/snort_upgrade.txt
-- Installing: /usr/local/share/doc/snort/snort_upgrade.text
-- Installing: /usr/local/share/doc/snort/snort_devel.txt
-- Installing: /usr/local/share/doc/snort/extending.txt
-- Installing: /usr/local/share/doc/snort/style.txt
-- Installing: /usr/local/share/doc/snort/versions.txt
