┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ sudo snort -T -c /usr/local/etc/snort/snort.lua
[sudo] password for kali: 
--------------------------------------------------
o")~   Snort++ 3.12.2.0
--------------------------------------------------
Loading /usr/local/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        output
        rpc_decode
        ips
        classifications
        references
        wizard
        file_inspect
        ftp_data
        ftp_server
        smtp
        port_scan
        gtp_inspect
        dce_http_server
        stream_file
        imap
        netflow
        iec104
        normalizer
        pop
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        sip
        stream
        stream_ip
        stream_icmp
        stream_tcp
        stream_udp
        stream_user
        arp_spoof
        back_orifice
        dns
        socks
        ssh
        ssl
        telnet
        cip
        dnp3
        mms
        modbus
        opcua
        s7commplus
        dce_smb
        dce_tcp
        dce_udp
        dce_http_proxy
        ftp_client
        http_inspect
        http2_inspect
        file_policy
        js_norm
        appid
        binder
Finished /usr/local/etc/snort/snort.lua:
Loading file_inspect.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_inspect.rules_file:
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               1     219       0     219    /usr/local/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 219
               text rules: 219
            option chains: 219
            chain headers: 1
--------------------------------------------------
service rule counts          to-srv  to-cli
                  file_id:      219     219
                    total:      219     219
--------------------------------------------------
fast pattern groups
                to_server: 1
                to_client: 1
--------------------------------------------------
search engine (ac_bnfa)
appid: MaxRss diff: 2816
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.

Snort successfully validated the configuration (with 0 warnings).
o")~   Snort exiting
┌──(kali㉿kali)-[~]
└─$ sudo nano /usr/local/etc/snort/snort.lua
[sudo] password for kali: 
                                                                           
┌──(kali㉿kali)-[~]
└─$ sudo snort -T -c /usr/local/etc/snort/snort.lua
--------------------------------------------------
o")~   Snort++ 3.12.2.0
--------------------------------------------------
Loading /usr/local/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        ips
        classifications
        references
        wizard
        active
        file_inspect
        ftp_data
        output
        dce_tcp
        host_tracker
        network
        process
        rpc_decode
        alerts
        daq
        host_cache
        hosts
        packets
        search_engine
        stream
        stream_ip
        stream_icmp
        stream_tcp
        stream_udp
        stream_user
        stream_file
        arp_spoof
        back_orifice
        dns
        imap
        netflow
        normalizer
        pop
        sip
        socks
        ssh
        ssl
        telnet
        cip
        dnp3
        iec104
        mms
        modbus
        opcua
        s7commplus
        dce_smb
        dce_udp
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_server
        ftp_client
        http_inspect
        http2_inspect
        file_policy
        js_norm
        appid
        binder
        decode
Finished /usr/local/etc/snort/snort.lua:
Loading file_inspect.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_inspect.rules_file:
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               1     219       0     219    /usr/local/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 219
               text rules: 219
            option chains: 219
            chain headers: 1
--------------------------------------------------
service rule counts          to-srv  to-cli
                  file_id:      219     219
                    total:      219     219
--------------------------------------------------
fast pattern groups
                to_server: 1
                to_client: 1
--------------------------------------------------
search engine (ac_bnfa)
appid: MaxRss diff: 2816
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.

Snort successfully validated the configuration (with 0 warnings).
o")~   Snort exiting









──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ ip -br addr
lo               UNKNOWN        127.0.0.1/8 ::1/128 
eth0             UP             192.168.56.101/24 fe80::2fbf:958f:3f7d:2283/64 
eth1             UP             10.0.3.15/24 fe80::59e1:391b:cba2:1bfb/64 
docker0          DOWN           172.17.0.1/16 







┌──(kali㉿kali)-[~]
└─$ sudo snort -i eth0 -c /usr/local/etc/snort/snort.lua
--------------------------------------------------
o")~   Snort++ 3.12.2.0
--------------------------------------------------
Loading /usr/local/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        ips
        references
        binder
        wizard
        stream_file
        arp_spoof
        back_orifice
        dns
        netflow
        normalizer
        pop
        rpc_decode
        sip
        socks
        ssh
        ssl
        telnet
        cip
        dnp3
        iec104
        output
        modbus
        opcua
        s7commplus
        dce_tcp
        dce_udp
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_server
        ftp_client
        ftp_data
        http_inspect
        appid
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        process
        search_engine
        js_norm
        file_policy
        file_inspect
        http2_inspect
        stream
        stream_ip
        stream_icmp
        stream_tcp
        dce_smb
        mms
        imap
        stream_user
        stream_udp
        classifications
        packets
Finished /usr/local/etc/snort/snort.lua:
Loading file_inspect.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_inspect.rules_file:
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               1     219       0     219    /usr/local/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 219
               text rules: 219
            option chains: 219
            chain headers: 1
--------------------------------------------------
service rule counts          to-srv  to-cli
                  file_id:      219     219
                    total:      219     219
--------------------------------------------------
fast pattern groups
                to_server: 1
                to_client: 1
--------------------------------------------------
search engine (ac_bnfa)
                instances: 2
                 patterns: 438
            pattern chars: 2602
               num states: 1832
         num match states: 392
             memory scale: KB
             total memory: 71.2812
           pattern memory: 19.6484
        match list memory: 28.4375
        transition memory: 22.9453
appid: MaxRss diff: 2984
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.
Commencing packet processing
Retry queue interval is: 200 ms
++ [0] eth0
^C** caught int signal
== stopping
-- [0] eth0                                            
--------------------------------------------------
Packet Statistics
--------------------------------------------------
daq
                 received: 73
                 analyzed: 73
                    allow: 73
                 rx_bytes: 7899
--------------------------------------------------
codec
                    total: 73           (100.000%)
                 discards: 1            (  1.370%)
                      arp: 7            (  9.589%)
                      eth: 73           (100.000%)
                    icmp4: 62           ( 84.932%)
                     ipv4: 66           ( 90.411%)
                      udp: 4            (  5.479%)
--------------------------------------------------
Module Statistics
--------------------------------------------------
ac_full
                 searches: 3
                  matches: 557
                    bytes: 1036
--------------------------------------------------
appid
                  packets: 65
        processed_packets: 65
           total_sessions: 3
       service_cache_adds: 3
             bytes_in_use: 504
             items_in_use: 3
--------------------------------------------------
arp_spoof
                  packets: 7
--------------------------------------------------
back_orifice
                  packets: 3
--------------------------------------------------
binder
              raw_packets: 7
                new_flows: 3
                 inspects: 10
--------------------------------------------------
detection
                 analyzed: 73
--------------------------------------------------
port_scan
                  packets: 66
                 trackers: 8
--------------------------------------------------
stream
                    flows: 3
             total_prunes: 1
idle_prunes_proto_timeout: 1
       udp_timeout_prunes: 1
--------------------------------------------------
stream_icmp
                 sessions: 1
                      max: 1
                  created: 1
                 released: 1
--------------------------------------------------
stream_udp
                 sessions: 2
                      max: 2
                  created: 2
                 released: 2
              total_bytes: 1007
--------------------------------------------------
udp
        bad_udp4_checksum: 1
--------------------------------------------------
wizard
                udp_scans: 2
               udp_misses: 2
--------------------------------------------------
Appid Statistics
--------------------------------------------------
detected apps and services
              Application: Services   Clients    Users      Payloads   Misc       Referred  
                  unknown: 2          0          0          0          0          0         
--------------------------------------------------
Summary Statistics
--------------------------------------------------
process
                  signals: 1
--------------------------------------------------
timing
                  runtime: 00:06:20
                  seconds: 380.937123
o")~   Snort exiting









┌──(kali㉿kali)-[~]
└─$ sudo snort -i eth0 -A alert_fast -c /usr/local/etc/snort/snort.lua
[sudo] password for kali: 
--------------------------------------------------
o")~   Snort++ 3.12.2.0
--------------------------------------------------
Loading /usr/local/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        stream
        stream_icmp
        stream_tcp
        stream_udp
        arp_spoof
        back_orifice
        netflow
        rpc_decode
        sip
        ssl
        cip
        output
        ips
        classifications
        references
        binder
        wizard
        appid
        js_norm
        file_policy
        file_inspect
        http2_inspect
        http_inspect
        ftp_data
        ftp_client
        ftp_server
        smtp
        port_scan
        gtp_inspect
        dce_http_server
        dce_http_proxy
        dce_udp
        dce_tcp
        dce_smb
        s7commplus
        opcua
        modbus
        mms
        iec104
        dnp3
        telnet
        ssh
        socks
        pop
        normalizer
        imap
        dns
        stream_file
        stream_user
        stream_ip
Finished /usr/local/etc/snort/snort.lua:
Loading file_inspect.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_inspect.rules_file:
Loading ips.rules:
Loading /usr/local/etc/snort/local.rules:
Finished /usr/local/etc/snort/local.rules:
Finished ips.rules:
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               1     220       0     220    /usr/local/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 220
               text rules: 220
            option chains: 220
            chain headers: 2
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any       0       0       1       0
   total       0       0       1       0
--------------------------------------------------
service rule counts          to-srv  to-cli
                  file_id:      219     219
                    total:      219     219
--------------------------------------------------
fast pattern groups
                to_server: 1
                to_client: 1
--------------------------------------------------
search engine (ac_bnfa)
                instances: 2
                 patterns: 438
            pattern chars: 2602
               num states: 1832
         num match states: 392
             memory scale: KB
             total memory: 71.2812
           pattern memory: 19.6484
        match list memory: 28.4375
        transition memory: 22.9453
appid: MaxRss diff: 3072
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.
Commencing packet processing
Retry queue interval is: 200 ms
++ [0] eth0
07/23-07:02:00.618392 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:00.618451 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:01.606634 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:01.606664 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:02.604140 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:02.604169 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:03.601138 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:03.601170 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:04.599676 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:04.599705 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:05.596745 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:05.596778 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:06.594461 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:06.594493 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:07.594145 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:07.594175 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:08.591221 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:08.591262 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:09.591038 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:09.591073 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:10.588553 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:10.588583 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:11.585253 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:11.585292 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:12.583327 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:12.583359 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:13.582182 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:13.582209 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:14.581157 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:14.581186 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:15.579234 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:15.579273 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:16.577283 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:16.577316 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:17.575909 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:17.575943 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:18.573098 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:18.573129 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:19.570382 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:19.570418 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:20.578536 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:20.578564 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:21.593946 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:21.593988 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:22.600162 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:22.600228 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:23.594787 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:23.594821 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:24.592078 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:24.592115 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:25.599025 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:25.599064 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:26.595801 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:26.595828 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:27.593045 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:27.593074 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:28.590669 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:28.590696 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:29.588248 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:29.588284 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:30.585996 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:30.586055 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:31.589547 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:31.589591 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:32.587690 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:32.587727 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:33.585226 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:33.585266 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:34.582794 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:34.582821 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:35.581696 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:35.581739 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:36.589265 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:36.589292 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:37.587871 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:37.587902 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:38.585821 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:38.585852 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:39.595068 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:39.595106 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:40.592773 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:40.592802 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:41.591774 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:41.591800 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:42.589122 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:42.589149 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:43.587203 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:43.587231 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:44.594003 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:44.594045 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:45.593975 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:45.594017 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:46.591828 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:46.591859 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:47.589004 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:47.589107 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:48.586561 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:48.586593 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:49.585045 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:49.585075 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:50.583175 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:50.583215 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:51.582436 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:51.582487 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:52.589164 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:52.589197 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:53.587729 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:53.587755 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:54.586536 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:54.586576 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:55.583852 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:55.583883 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:56.582579 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:56.582610 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:57.590321 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:57.590355 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:58.589242 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:58.589272 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:02:59.587506 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:02:59.587536 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102
07/23-07:03:00.595575 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.102 -> 192.168.56.101
07/23-07:03:00.595611 [**] [1:1000001:1] "ICMP Ping Detected" [**] [Priority: 0] {ICMP} 192.168.56.101 -> 192.168.56.102












┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--network host \
--entrypoint /home/snorty/snort3/bin/snort \
-v ~/snort-config/snort:/home/snorty/snort3/etc/snort \
-v ~/snort-config/rules:/home/snorty/snort3/etc/rules \
ciscotalos/snort3 \
-c /home/snorty/snort3/etc/snort/snort.lua \
-i eth0
[sudo] password for kali: 
--------------------------------------------------
o")~   Snort++ 3.10.0.0
--------------------------------------------------
Loading /home/snorty/snort3/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        so_proxy
        dce_tcp
        dce_udp
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_client
        ftp_data
        http_inspect
        http2_inspect
        file_policy
        js_norm
        appid
        wizard
        binder
        references
        classifications
        ips
        file_id
        ftp_server
        dce_smb
        s7commplus
        opcua
        modbus
        mms
        iec104
        dnp3
        cip
        telnet
        ssl
        ssh
        sip
        rpc_decode
        pop
        normalizer
        netflow
        imap
        dns
        back_orifice
        arp_spoof
        stream_file
        stream_user
        stream_udp
        stream_tcp
        stream_icmp
        stream_ip
        stream
        trace
        output
        active
        alerts
Finished /home/snorty/snort3/etc/snort/snort.lua:
Loading file_id.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_id.rules_file:
Loading ips.rules:
Loading /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished ips.rules:
--------------------------------------------------
pcre counts
               pcre_rules: 1080
              pcre_native: 1080
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               0    4236       0    4236    /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 4236
               text rules: 4236
            option chains: 4236
            chain headers: 288
                 flowbits: 48
     flowbits not checked: 23
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any     472      58     147      22
     src     169      15       0       0
     dst     775     150       0       0
    both       6      11       0       0
   total    1422     234     147      22
--------------------------------------------------
service rule counts          to-srv  to-cli
                   dcerpc:       72      20
                     dhcp:        2       2
                      dns:       28       7
                  file_id:      219     219
                      ftp:       90       4
                 ftp-data:        1      94
                     http:     2084     253
                    http2:     2084     253
                    http3:     2084     253
                     imap:       35     115
                      irc:        5       2
                 kerberos:        3       0
                     ldap:        0       1
                    mysql:        3       0
              netbios-dgm:        1       1
               netbios-ns:        4       3
              netbios-ssn:       69      17
                     nntp:        2       0
                     pop3:       23     115
                      rdp:        5       0
                      sip:        5       5
                     smtp:      129       2
                     snmp:       18       7
                     ssdp:        3       0
                      ssl:       20      42
                   sunrpc:       68       4
                   telnet:       12       6
                     tftp:        1       0
                     wins:        1       0
                    total:     7071    1425
--------------------------------------------------
fast pattern groups
                      src: 114
                      dst: 312
                      any: 8
                to_server: 69
                to_client: 48
--------------------------------------------------
search engine (ac_bnfa)
                instances: 334
                 patterns: 10779
            pattern chars: 175198
               num states: 123200
         num match states: 10502
             memory scale: MB
             total memory: 3.68016
           pattern memory: 0.57795
        match list memory: 1.33499
        transition memory: 1.Couldn't start DAQ instance (eth0): socket: Operation not permitted (-1)
Analyzer: Failed to start DAQ instance
72644
        fast pattern only: 7097
appid: MaxRss diff: 3072
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.
Commencing packet processing
Retry queue interval is: 200 ms
++ [0] eth0
-- [0] eth0
--------------------------------------------------
Packet Statistics
--------------------------------------------------
Module Statistics
--------------------------------------------------
Summary Statistics
--------------------------------------------------
timing
                  runtime: 00:00:00
                  seconds: 0.120630
o")~   Snort exiting
                                                                           
┌──(kali㉿kali)-[~]
└─$ 
                                                                           
┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--network host \
--cap-add=NET_ADMIN \
--cap-add=NET_RAW \
--entrypoint /home/snorty/snort3/bin/snort \
-v ~/snort-config/snort:/home/snorty/snort3/etc/snort \
-v ~/snort-config/rules:/home/snorty/snort3/etc/rules \
ciscotalos/snort3 \
-c /home/snorty/snort3/etc/snort/snort.lua \
-i eth0 \
-A alert_fast
--------------------------------------------------
o")~   Snort++ 3.10.0.0
--------------------------------------------------
Loading /home/snorty/snort3/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        output
        ips
        classifications
        references
        binder
        wizard
        appid
        js_norm
        file_policy
        file_id
        http2_inspect
        http_inspect
        packets
        gtp_inspect
        dce_http_proxy
        dce_udp
        normalizer
        netflow
        imap
        dns
        arp_spoof
        stream_user
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        process
        search_engine
        so_proxy
        stream
        stream_ip
        stream_icmp
        stream_tcp
        stream_udp
        stream_file
        back_orifice
        pop
        rpc_decode
        sip
        ssh
        ssl
        telnet
        cip
        dnp3
        iec104
        mms
        modbus
        opcua
        s7commplus
        dce_smb
        dce_tcp
        dce_http_server
        port_scan
        smtp
        ftp_server
        ftp_client
        ftp_data
        trace
Finished /home/snorty/snort3/etc/snort/snort.lua:
Loading file_id.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_id.rules_file:
Loading ips.rules:
Loading /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished ips.rules:
--------------------------------------------------
pcre counts
               pcre_rules: 1080
              pcre_native: 1080
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               0    4236       0    4236    /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 4236
               text rules: 4236
            option chains: 4236
            chain headers: 288
                 flowbits: 48
     flowbits not checked: 23
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any     472      58     147      22
     src     169      15       0       0
     dst     775     150       0       0
    both       6      11       0       0
   total    1422     234     147      22
--------------------------------------------------
service rule counts          to-srv  to-cli
                   dcerpc:       72      20
                     dhcp:        2       2
                      dns:       28       7
                  file_id:      219     219
                      ftp:       90       4
                 ftp-data:        1      94
                     http:     2084     253
                    http2:     2084     253
                    http3:     2084     253
                     imap:       35     115
                      irc:        5       2
                 kerberos:        3       0
                     ldap:        0       1
                    mysql:        3       0
              netbios-dgm:        1       1
               netbios-ns:        4       3
              netbios-ssn:       69      17
                     nntp:        2       0
                     pop3:       23     115
                      rdp:        5       0
                      sip:        5       5
                     smtp:      129       2
                     snmp:       18       7
                     ssdp:        3       0
                      ssl:       20      42
                   sunrpc:       68       4
                   telnet:       12       6
                     tftp:        1       0
                     wins:        1       0
                    total:     7071    1425
--------------------------------------------------
fast pattern groups
                      src: 114
                      dst: 312
                      any: 8
                to_server: 69
                to_client: 48
--------------------------------------------------
search engine (ac_bnfa)
                instances: 334
                 patterns: 10779
            pattern chars: 175198
               num states: 123200
         num match states: 10502
             memory scale: MB
             total memory: 3.68016
           pattern memory: 0.57795
        match list memory: 1.33499
        transition memory: 1.Couldn't start DAQ instance (eth0): socket: Operation not permitted (-1)
Analyzer: Failed to start DAQ instance
72644
        fast pattern only: 7097
appid: MaxRss diff: 3328
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.
Commencing packet processing
Retry queue interval is: 200 ms
++ [0] eth0
-- [0] eth0
--------------------------------------------------
Packet Statistics
--------------------------------------------------
Module Statistics
--------------------------------------------------
Summary Statistics
--------------------------------------------------
timing
                  runtime: 00:00:00
                  seconds: 0.016878
o")~   Snort exiting
                                                                           
┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--network host \
--cap-add=NET_ADMIN \
--cap-add=NET_RAW \
--entrypoint /bin/bash \
ciscotalos/snort3 \
-c "id && capsh --print"
uid=1000(snorty) gid=1000(snorty) groups=1000(snorty)
/bin/bash: line 1: capsh: command not found
                                                                           
┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--user root \
--network host \
--cap-add=NET_ADMIN \
--cap-add=NET_RAW \
--entrypoint /home/snorty/snort3/bin/snort \
-v ~/snort-config/snort:/home/snorty/snort3/etc/snort \
-v ~/snort-config/rules:/home/snorty/snort3/etc/rules \
ciscotalos/snort3 \
-c /home/snorty/snort3/etc/snort/snort.lua \
-i eth0 \
-A alert_fast
--------------------------------------------------
o")~   Snort++ 3.10.0.0
--------------------------------------------------
Loading /home/snorty/snort3/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        ips
        output
        classifications
        references
        binder
        wizard
        appid
        js_norm
        file_policy
        file_id
        http2_inspect
        ftp_data
        ftp_server
        gtp_inspect
        dce_http_proxy
        dce_tcp
        trace
        host_cache
        stream
        active
        alerts
        daq
        decode
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        so_proxy
        stream_ip
        stream_icmp
        stream_tcp
        stream_udp
        stream_user
        stream_file
        arp_spoof
        back_orifice
        dns
        imap
        netflow
        normalizer
        pop
        rpc_decode
        sip
        ssh
        ssl
        telnet
        cip
        dnp3
        iec104
        mms
        modbus
        opcua
        s7commplus
        dce_smb
        dce_udp
        dce_http_server
        port_scan
        smtp
        ftp_client
        http_inspect
Finished /home/snorty/snort3/etc/snort/snort.lua:
Loading file_id.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_id.rules_file:
Loading ips.rules:
Loading /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished ips.rules:
--------------------------------------------------
pcre counts
               pcre_rules: 1080
              pcre_native: 1080
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               0    4236       0    4236    /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 4236
               text rules: 4236
            option chains: 4236
            chain headers: 288
                 flowbits: 48
     flowbits not checked: 23
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any     472      58     147      22
     src     169      15       0       0
     dst     775     150       0       0
    both       6      11       0       0
   total    1422     234     147      22
--------------------------------------------------
service rule counts          to-srv  to-cli
                   dcerpc:       72      20
                     dhcp:        2       2
                      dns:       28       7
                  file_id:      219     219
                      ftp:       90       4
                 ftp-data:        1      94
                     http:     2084     253
                    http2:     2084     253
                    http3:     2084     253
                     imap:       35     115
                      irc:        5       2
                 kerberos:        3       0
                     ldap:        0       1
                    mysql:        3       0
              netbios-dgm:        1       1
               netbios-ns:        4       3
              netbios-ssn:       69      17
                     nntp:        2       0
                     pop3:       23     115
                      rdp:        5       0
                      sip:        5       5
                     smtp:      129       2
                     snmp:       18       7
                     ssdp:        3       0
                      ssl:       20      42
                   sunrpc:       68       4
                   telnet:       12       6
                     tftp:        1       0
                     wins:        1       0
                    total:     7071    1425
--------------------------------------------------
fast pattern groups
                      src: 114
                      dst: 312
                      any: 8
                to_server: 69
                to_client: 48
--------------------------------------------------
search engine (ac_bnfa)
                instances: 334
                 patterns: 10779
            pattern chars: 175198
               num states: 123200
         num match states: 10502
             memory scale: MB
             total memory: 3.68016
           pattern memory: 0.57795
        match list memory: 1.33499
        transition memory: 1.72644
        fast pattern only: 7097
appid: MaxRss diff: 3072
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.
Commencing packet processing
Retry queue interval is: 200 ms
++ [0] eth0
07/22-15:53:21.094320 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:21.094320 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:21.094320 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:21.095258 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:53:22.095721 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:22.095721 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:22.095721 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:22.096545 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:53:23.100299 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:23.100299 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:23.100299 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:23.101214 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:53:24.102085 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:24.102085 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:24.102085 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:53:24.103434 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:53:53.636057 [**] [1:1418:19] "PROTOCOL-SNMP request tcp" [**] [Classification: Attempted Information Leak] [Priority: 2] {TCP} 192.168.56.101:59231 -> 192.168.56.102:161
07/22-15:53:54.003732 [**] [1:1421:19] "PROTOCOL-SNMP AgentX/tcp request" [**] [Classification: Attempted Information Leak] [Priority: 2] {TCP} 192.168.56.101:59231 -> 192.168.56.102:705
** caught term signal
== stopping
07/22-15:55:05.670408 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:05.670408 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:05.670408 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:05.678335 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:55:06.672599 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:06.672599 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:06.672599 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:06.673671 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:55:07.673242 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:07.673242 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:07.673242 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:07.674319 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
07/22-15:55:08.673693 [**] [1:366:11] "PROTOCOL-ICMP PING Unix" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:08.673693 [**] [1:29456:3] "PROTOCOL-ICMP Unusual PING detected" [**] [Classification: Information Leak] [Priority: 2] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:08.673693 [**] [1:384:8] "PROTOCOL-ICMP PING" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.101 -> 192.168.56.102
07/22-15:55:08.675161 [**] [1:408:8] "PROTOCOL-ICMP Echo Reply" [**] [Classification: Misc activity] [Priority: 3] {ICMP} 192.168.56.102 -> 192.168.56.101
-- [0] eth0
--------------------------------------------------
Packet Statistics
--------------------------------------------------
daq
                 received: 2064
                 analyzed: 2063
                    allow: 2063
                 rx_bytes: 124343
--------------------------------------------------
codec
                    total: 2063         (100.000%)
                 discards: 2            (  0.097%)
                      arp: 17           (  0.824%)
                      eth: 2063         (100.000%)
                    icmp4: 16           (  0.776%)
                     ipv4: 2046         ( 99.176%)
                      tcp: 2023         ( 98.061%)
                      udp: 7            (  0.339%)
--------------------------------------------------
Module Statistics
--------------------------------------------------
ac_bnfa
                 searches: 23
                  matches: 37
                    bytes: 3791
--------------------------------------------------
ac_full
                 searches: 5
                  matches: 1114
                    bytes: 1828
--------------------------------------------------
appid
                  packets: 2044
        processed_packets: 2044
           total_sessions: 1005
       service_cache_adds: 3
             bytes_in_use: 504
             items_in_use: 3
--------------------------------------------------
arp_spoof
                  packets: 17
--------------------------------------------------
back_orifice
                  packets: 5
--------------------------------------------------
binder
              raw_packets: 17
                new_flows: 1003
                 inspects: 1020
--------------------------------------------------
detection
                 analyzed: 2063
               hard_evals: 2107
             raw_searches: 23
             pkt_searches: 23
                   alerts: 34
             total_alerts: 34
                   logged: 34
--------------------------------------------------
ips_actions
                    alert: 34
--------------------------------------------------
port_scan
                  packets: 2046
                 trackers: 10
--------------------------------------------------
search_engine
               max_queued: 2
            total_flushed: 37
            total_inserts: 37
             total_unique: 37
     non_qualified_events: 2118
         qualified_events: 26
--------------------------------------------------
stream
                    flows: 1003
             total_prunes: 997
idle_prunes_proto_timeout: 20
            closed_prunes: 977
       tcp_timeout_prunes: 20
--------------------------------------------------
stream_icmp
                 sessions: 1
                      max: 1
                  created: 1
                 released: 1
--------------------------------------------------
stream_tcp
                 sessions: 1000
                      max: 1000
                  created: 1000
                 released: 1000
             instantiated: 1000
                   setups: 1000
             syn_trackers: 1000
                     syns: 1000
                 syn_acks: 23
                     rsts: 1000
          rsts_ok_rfc5961: 23
              rsts_ack_ok: 977
--------------------------------------------------
stream_udp
                 sessions: 2
                      max: 2
                  created: 4
                 released: 4
                 timeouts: 2
              total_bytes: 1799
--------------------------------------------------
udp
        bad_udp4_checksum: 2
--------------------------------------------------
wizard
                udp_scans: 2
               udp_misses: 2
--------------------------------------------------
Appid Statistics
--------------------------------------------------
detected apps and services
              Application: Services   Clients    Users      Payloads   Misc       Referred  
                  unknown: 4          0          0          0          0          0         
--------------------------------------------------
Summary Statistics
--------------------------------------------------
process
                  signals: 1
--------------------------------------------------
timing
                  runtime: 00:09:09
                  seconds: 549.513757
                 pkts/sec: 4
o")~   Snort exiting










┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--user root \
--network host \
--cap-add=NET_ADMIN \
--cap-add=NET_RAW \
--entrypoint /home/snorty/snort3/bin/snort \
-v ~/snort-config/snort:/home/snorty/snort3/etc/snort \
-v ~/snort-config/rules:/home/snorty/snort3/etc/rules \
ciscotalos/snort3 \
-c /home/snorty/snort3/etc/snort/snort.lua \
-i eth0 \
-A alert_fast
[sudo] password for kali: 
--------------------------------------------------
o")~   Snort++ 3.10.0.0
--------------------------------------------------
Loading /home/snorty/snort3/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        ips
        file_id
        stream_udp
        stream_user
        stream_file
        arp_spoof
        back_orifice
        dns
        imap
        netflow
        normalizer
        pop
        rpc_decode
        sip
        ssh
        telnet
        cip
        dnp3
        iec104
        mms
        modbus
        dce_smb
        dce_tcp
        dce_udp
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_server
        ftp_client
        ftp_data
        http2_inspect
        classifications
        file_policy
        js_norm
        appid
        wizard
        references
        binder
        http_inspect
        s7commplus
        opcua
        ssl
        stream_tcp
        stream_ip
        active
        alerts
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        so_proxy
        stream
        stream_icmp
        trace
        output
        daq
Finished /home/snorty/snort3/etc/snort/snort.lua:
Loading file_id.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_id.rules_file:
Loading ips.rules:
Loading /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished /home/snorty/snort3/etc/rules/snort3-community.rules:
Loading /home/snorty/snort3/etc/rules/local.rules:
Finished /home/snorty/snort3/etc/rules/local.rules:
Finished ips.rules:
--------------------------------------------------
pcre counts
               pcre_rules: 1080
              pcre_native: 1080
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               0    4237       0    4237    /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 4237
               text rules: 4237
            option chains: 4237
            chain headers: 288
                 flowbits: 48
     flowbits not checked: 23
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any     472      58     148      22
     src     169      15       0       0
     dst     775     150       0       0
    both       6      11       0       0
   total    1422     234     148      22
--------------------------------------------------
service rule counts          to-srv  to-cli
                   dcerpc:       72      20
                     dhcp:        2       2
                      dns:       28       7
                  file_id:      219     219
                      ftp:       90       4
                 ftp-data:        1      94
                     http:     2084     253
                    http2:     2084     253
                    http3:     2084     253
                     imap:       35     115
                      irc:        5       2
                 kerberos:        3       0
                     ldap:        0       1
                    mysql:        3       0
              netbios-dgm:        1       1
               netbios-ns:        4       3
              netbios-ssn:       69      17
                     nntp:        2       0
                     pop3:       23     115
                      rdp:        5       0
                      sip:        5       5
                     smtp:      129       2
                     snmp:       18       7
                     ssdp:        3       0
                      ssl:       20      42
                   sunrpc:       68       4
                   telnet:       12       6
                     tftp:        1       0
                     wins:        1       0
                    total:     7071    1425
--------------------------------------------------
fast pattern groups
                      src: 114
                      dst: 312
                      any: 8
                to_server: 69
                to_client: 48
--------------------------------------------------
search engine (ac_bnfa)
                instances: 334
                 patterns: 10779
            pattern chars: 175198
               num states: 123200
         num match states: 10502
             memory scale: MB
             total memory: 3.68                                                                           
┌──(kali㉿kali)-[~]
└─$ sudo docker run --rm \
--user root \
--network host \
--cap-add=NET_ADMIN \
--cap-add=NET_RAW \
--entrypoint /home/snorty/snort3/bin/snort \
-v ~/snort-config/snort:/home/snorty/snort3/etc/snort \
-v ~/snort-config/rules:/home/snorty/snort3/etc/rules \
ciscotalos/snort3 \
-c /home/snorty/snort3/etc/snort/snort.lua \
-i eth0 \
-v
--------------------------------------------------
o")~   Snort++ 3.10.0.0
--------------------------------------------------
Loading /home/snorty/snort3/etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        Lua Allowlist Keywords for /home/snorty/snort3/etc/snort/snort.lua:
                default_classifications, default_ftp_server, default_gtp,
                default_hi_port_scan, default_js_norm, default_js_norm_ident_ignore,
                default_js_norm_prop_ignore, default_low_port_scan, default_med_port_scan,
                default_references, default_smtp, default_variables, default_wizard,
                ftp_command_specs, gtp_v0_info, gtp_v0_msg, gtp_v1_info, gtp_v1_msg,
                gtp_v2_info, gtp_v2_msg, http_methods, icmp_hi_sweep, icmp_low_sweep,
                icmp_med_sweep, ip_hi_decoy, ip_hi_dist, ip_hi_proto, ip_hi_sweep,
                ip_low_decoy, ip_low_dist, ip_low_proto, ip_low_sweep, ip_med_decoy,
                ip_med_dist, ip_med_proto, ip_med_sweep, netflow_versions, sip_requests,
                smtp_default_alt_max_command_lines, tcp_hi_decoy, tcp_hi_dist, tcp_hi_ports,
                tcp_hi_sweep, tcp_low_decoy, tcp_low_dist, tcp_low_ports, tcp_low_sweep,
                tcp_med_decoy, tcp_med_dist, tcp_med_ports, tcp_med_sweep, telnet_commands,
                udp_hi_decoy, udp_hi_dist, udp_hi_ports, udp_hi_sweep, udp_low_decoy,
                udp_low_dist, udp_low_ports, udp_low_sweep, udp_med_decoy, udp_med_dist,
                udp_med_ports, udp_med_sweep
        trace
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        so_proxy
        output
        dce_smb
        dce_tcp
        pop
        telnet
        mms
        s7commplus
        imap
        dns
        sip
        opcua
        modbus
        iec104
        dnp3
        cip
        ssl
        ssh
        dce_udp
        rpc_decode
        normalizer
        netflow
        ips
        file_id
        back_orifice
        arp_spoof
        stream_file
        stream_user
        stream_udp
        stream_tcp
        stream_icmp
        stream_ip
        stream
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_server
        ftp_client
        ftp_data
        http_inspect
        http2_inspect
        file_policy
        js_norm
        appid
        wizard
        binder
        references
        classifications
Finished /home/snorty/snort3/etc/snort/snort.lua:
Loading file_id.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_id.rules_file:
Loading ips.rules:
Loading /home/snorty/snort3/etc/rules/snort3-community.rules:
Finished /home/snorty/snort3/etc/rules/snort3-community.rules:
Loading /home/snorty/snort3/etc/rules/local.rules:
Finished /home/snorty/snort3/etc/rules/local.rules:
Finished ips.rules:
--------------------------------------------------
pcre counts
               pcre_rules: 1080
              pcre_native: 1080
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               0    4237       0    4237    /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 4237
               text rules: 4237
            option chains: 4237
            chain headers: 288
                 flowbits: 48
     flowbits not checked: 23
--------------------------------------------------
port rule counts
             tcp     udp    icmp      ip
     any     472      58     148      22
     src     169      15       0       0
     dst     775     150       0       0
    both       6      11       0       0
   total    1422     234     148      22
--------------------------------------------------
service rule counts          to-srv  to-cli
                   dcerpc:       72      20
                     dhcp:        2       2
                      dns:       28       7
                  file_id:      219     219
                      ftp:       90       4
                 ftp-data:        1      94
                     http:     2084     253
                    http2:     2084     253
                    http3:     2084     253
                     imap:       35     115
                      irc:        5       2
                 kerberos:        3       0
                     ldap:        0       1
                    mysql:        3       0
              netbios-dgm:        1       1
               netbios-ns:        4       3
              netbios-ssn:       69      17
                     nntp:        2       0
                     pop3:       23     115
                      rdp:        5       0
                      sip:        5       5
                     smtp:      129       2
                     snmp:       18       7
                     ssdp:        3       0
                      ssl:       20      42
                   sunrpc:       68       4
                   telnet:       12       6
                     tftp:        1       0
                     wins:        1       0
                    total:     7071    1425
--------------------------------------------------
fast pattern groups
                      src: 114
                      dst: 312
                      any: 8
                to_server: 69
                to_client: 48
--------------------------------------------------
search engine (ac_bnfa)
                instances: 334
                 patterns: 10779
            pattern chars: 175198
               num states: 123200
         num match states: 10502
             memory scale: MB
             total memory: 3.68016
           pattern memory: 0.57795
        match list memory: 1.33499
        transition memory: 1.72644
        fast pattern only: 7097
AppId Lua-Detector Stats: control instance, odp detectors 0, custom detectors 0, total memory 50 kb
appid: MaxRss diff: 3256
appid: patterns loaded: 300
--------------------------------------------------
File Identification
--------------------------------------------------
file_id:
              enable_type: enabled
               type_depth: 1460
         enable_signature: disabled
     block_timeout_lookup: disabled
           enable_capture: disabled
           lookup_timeout: 2
         max_files_cached: 65536
       max_files_per_flow: 128
          show_data_depth: 100
               trace_type: disabled
          trace_signature: disabled
             trace_stream: disabled
--------------------------------------------------
Flow Tracking
--------------------------------------------------
stream:
            ip_frags_only: disabled
                max_flows: 476288
               max_aux_ip: 16
          pruning_timeout: 30
              prune_flows: 10
             require_3whs: -1 (disabled)
       drop_stale_packets: disabled
                 ip_cache: { idle_timeout = 180 }
                tcp_cache: { idle_timeout = 3600 }
                udp_cache: { idle_timeout = 180 }
               icmp_cache: { idle_timeout = 180 }
               user_cache: { idle_timeout = 180 }
               file_cache: { idle_timeout = 180 }
          allowlist_cache: { enable = false, move_on_excess = false }
--------------------------------------------------
Global Inspectors
--------------------------------------------------
appid:
         app_stats_period: 300
  app_stats_rollover_size: 20971520
       list_odp_detectors: disabled
    tp_appid_stats_enable: disabled
     tp_appid_config_dump: disabled
         log_all_sessions: disabled
                log_stats: disabled
                   memcap: 1048576
--------------------------------------------------
port_scan:
                   memcap: 10485760
                   protos: all
               scan_types: all
                alert_all: disabled
        include_midstream: disabled
               tcp_window: 90
               udp_window: 90
                ip_window: 90
              icmp_window: 90
--------------------------------------------------
so_proxy:
--------------------------------------------------
Network Policy : policy id 0 : /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
normalizer:
                      ip4: disabled
                      ip6: disabled
                    icmp4: disabled
                    icmp6: disabled
                      tcp: enabled
                      tcp: { ecn = disabled, block = disabled, rsv = disabled, pad = disabled, req_urg
                           = disabled, req_pay = disabled, req_urp = disabled, urp = disabled, ips =
                           enabled, trim = disabled }
--------------------------------------------------
Inspection Policy : policy id 0 : /home/snorty/snort3/etc/snort/snort.lua
--------------------------------------------------
arp_spoof:
--------------------------------------------------
back_orifice:
--------------------------------------------------
binder:
                 bindings:
                           { when = { role = server, proto = udp, ports = 53 },
                             use = { type = dns } }
                           { when = { role = server, proto = tcp, ports = 53 },
                             use = { type = dns } }
                           { when = { role = server, proto = tcp, ports = 111 },
                             use = { type = rpc_decode } }
                           { when = { role = server, proto = tcp, ports = 502 },
                             use = { type = modbus } }
                           { when = { role = server, proto = tcp, ports = 2123 2152 3386 },
                             use = { type = gtp_inspect } }
                           { when = { role = server, proto = tcp, ports = 2404 },
                             use = { type = iec104 } }
                           { when = { role = server, proto = udp, ports = 2222 },
                             use = { type = cip } }
                           { when = { role = server, proto = tcp, ports = 44818 },
                             use = { type = cip } }
                           { when = { service = dcerpc, proto = tcp },
                             use = { type = dce_tcp } }
                           { when = { service = dcerpc, proto = udp },
                             use = { type = dce_udp } }
                           { when = { service = netflow, proto = udp },
                             use = { type = netflow } }
                           { when = { service = netbios-ssn },
                             use = { type = dce_smb } }
                           { when = { service = dce_http_server },
                             use = { type = dce_http_server } }
                           { when = { service = dce_http_proxy },
                             use = { type = dce_http_proxy } }
                           { when = { service = cip },
                             use = { type = cip } }
                           { when = { service = dnp3 },
                             use = { type = dnp3 } }
                           { when = { service = dns },
                             use = { type = dns } }
                           { when = { service = ftp },
                             use = { type = ftp_server } }
                           { when = { service = ftp-data },
                             use = { type = ftp_data } }
                           { when = { service = gtp },
                             use = { type = gtp_inspect } }
                           { when = { service = imap },
                             use = { type = imap } }
                           { when = { service = http },
                             use = { type = http_inspect } }
                           { when = { service = http2 },
                             use = { type = http2_inspect } }
                           { when = { service = iec104 },
                             use = { type = iec104 } }
                           { when = { service = mms },
                             use = { type = mms } }
                           { when = { service = modbus },
                             use = { type = modbus } }
                           { when = { service = opcua },
                             use = { type = opcua } }
                           { when = { service = pop3 },
                             use = { type = pop } }
                           { when = { service = ssh },
                             use = { type = ssh } }
                           { when = { service = sip },
                             use = { type = sip } }
                           { when = { service = smtp },
                             use = { type = smtp } }
                           { when = { service = ssl },
                             use = { type = ssl } }
                           { when = { service = sunrpc },
                             use = { type = rpc_decode } }
                           { when = { service = s7commplus },
                             use = { type = s7commplus } }
                           { when = { service = telnet },
                             use = { type = telnet } }
                           { when = { },
                             use = { type = wizard } }
--------------------------------------------------
cip:
        embedded_cip_path: 0 183
      unconnected_timeout: 300
      max_cip_connections: 100
 max_unconnected_messages: 100
--------------------------------------------------
dce_http_proxy:
--------------------------------------------------
dce_http_server:
--------------------------------------------------
dce_smb:
             limit_alerts: enabled
           disable_defrag: disabled
             max_frag_len: 65535
                   policy: WinXP
     reassemble_threshold: 0
   smb_fingerprint_policy: disabled
            smb_max_chain: 3
         smb_max_compound: 3
       valid_smb_versions: all
           smb_file_depth: 16384
       smb_invalid_shares: none
          smb_legacy_mode: disabled
           smb_max_credit: 8192
--------------------------------------------------
dce_tcp:
             limit_alerts: enabled
           disable_defrag: disabled
             max_frag_len: 65535
                   policy: WinXP
     reassemble_threshold: 0
--------------------------------------------------
dce_udp:
             limit_alerts: enabled
           disable_defrag: disabled
             max_frag_len: 65535
--------------------------------------------------
dnp3:
                check_crc: disabled
--------------------------------------------------
dns:
         publish_response: 0
--------------------------------------------------
ftp_client:
                   bounce: disabled
 ignore_telnet_erase_cmds: disabled
             max_resp_len: 4294967295
              telnet_cmds: disabled
--------------------------------------------------
ftp_data:
--------------------------------------------------
ftp_server:
          check_encrypted: disabled
        def_max_param_len: 100
        encrypted_traffic: disabled
         ignore_data_chan: disabled
 ignore_telnet_erase_cmds: disabled
              telnet_cmds: disabled
               print_cmds: disabled
--------------------------------------------------
gtp_inspect:
--------------------------------------------------
http2_inspect:
 concurrent_streams_limit: 100
  settings_max_frame_size: 16777215
--------------------------------------------------
http_inspect:
            request_depth: -1 (unlimited)
           response_depth: -1 (unlimited)
     partial_depth_header: 0 (disabled)
       partial_depth_body: 0 (disabled)
                    unzip: enabled
            normalize_utf: enabled
           decompress_pdf: disabled
           decompress_swf: disabled
           decompress_zip: disabled
           decompress_vba: disabled
          max_mime_attach: 5
         script_detection: disabled
     normalize_javascript: disabled
max_javascript_whitespaces: 200
                percent_u: disabled
                     utf8: enabled
           utf8_bare_byte: disabled
              iis_unicode: disabled
    iis_unicode_code_page: 1252
        iis_double_decode: enabled
      oversize_dir_length: 300
       backslash_to_slash: enabled
            plus_to_space: enabled
            simplify_path: enabled
              xff_headers: x-forwarded-for true-client-ip
request_body_app_detection: enabled
--------------------------------------------------
iec104:
--------------------------------------------------
imap:
         b64_decode_depth: -1 (unlimited)
          qp_decode_depth: -1 (unlimited)
          uu_decode_depth: -1 (unlimited)
      bitenc_decode_depth: -1 (unlimited)
           decompress_pdf: disabled
           decompress_swf: disabled
           decompress_zip: disabled
           decompress_vba: disabled
   decompress_buffer_size: 100000
--------------------------------------------------
mms:
--------------------------------------------------
modbus:
--------------------------------------------------
netflow:
              flow_memcap: 0
          template_memcap: 0
           update_timeout: 3600
--------------------------------------------------
opcua:
--------------------------------------------------
pop:
         b64_decode_depth: -1 (unlimited)
          qp_decode_depth: -1 (unlimited)
          uu_decode_depth: -1 (unlimited)
      bitenc_decode_depth: -1 (unlimited)
           decompress_pdf: disabled
           decompress_swf: disabled
           decompress_zip: disabled
           decompress_vba: disabled
   decompress_buffer_size: 100000
--------------------------------------------------
rpc_decode:
--------------------------------------------------
s7commplus:
--------------------------------------------------
sip:
      ignore_call_channel: disabled
          max_call_id_len: 256
          max_contact_len: 256
          max_content_len: 1024
              max_dialogs: 4
             max_from_len: 256
     max_request_name_len: 20
               max_to_len: 256
              max_uri_len: 256
              max_via_len: 1024
                  methods: invite cancel ack bye register options refer subscribe update join info
                           message notify prack publish replace
              sip_timeout: 0
        sip_media_timeout: 0
       sip_invite_timeout: 0
   sip_disconnect_timeout: 0
--------------------------------------------------
smtp:
                normalize: none
           normalize_cmds: ATRN AUTH BDAT DATA DEBUG EHLO EMAL ESAM ESND ESOM ETRN EVFY EXPN HELO HELP
                           IDENT MAIL NOOP ONEX QUEU QUIT RCPT RSET SAML SEND STARTTLS SOML TICK TIME
                           TURN TURNME VERB VRFY X-EXPS XADR XAUTH XCIR XEXCH50 XGEN XLICENSE
                           X-LINK2STATE XQUE XSTA XTRN XUSR CHUNKING X-ADAT X-DRCP X-ERCP X-EXCH50
          ignore_tls_data: disabled
     max_command_line_len: 512
 alt_max_command_line_len: { {ATRN, 255}, {AUTH, 246}, {BDAT, 255}, {DATA, 246}, {DEBUG, 255}, {EHLO,
                           500}, {EMAL, 255}, {ESAM, 255}, {ESND, 255}, {ESOM, 255}, {ETRN, 500},
                           {EVFY, 255}, {EXPN, 255}, {HELO, 500}, {HELP, 500}, {IDENT, 255}, {MAIL,
                           260}, {NOOP, 255}, {ONEX, 246}, {QUEU, 246}, {QUIT, 246}, {RCPT, 300},
                           {RSET, 255}, {SAML, 246}, {SEND, 246}, {SIZE, 255}, {STARTTLS, 246}, {SOML,
                           246}, {TICK, 246}, {TIME, 246}, {TURN, 246}, {TURNME, 246}, {VERB, 246},
                           {VRFY, 255}, {X-EXPS, 246}, {XADR, 246}, {XAUTH, 246}, {XCIR, 246},
                           {XEXCH50, 246}, {XGEN, 246}, {XLICENSE, 246}, {X-LINK2STATE, 246}, {XQUE,
                           246}, {XSTA, 246}, {XTRN, 246}, {XUSR, 246} }
      max_header_line_len: 1000
max_auth_command_line_len: 1000
 max_response_line_length: 512
              xlink2state: alert
             invalid_cmds: none
                auth_cmds: AUTH X-EXPS XAUTH
         binary_data_cmds: BDAT XEXCH50
                data_cmds: DATA
               valid_cmds: ATRN AUTH BDAT DATA DEBUG EHLO EMAL ESAM ESND ESOM ETRN EVFY EXPN HELO HELP
                           IDENT MAIL NOOP ONEX QUEU QUIT RCPT RSET SAML SEND SIZE STARTTLS SOML TICK
                           TIME TURN TURNME VERB VRFY X-EXPS XADR XAUTH XCIR XEXCH50 XGEN XLICENSE
                           X-LINK2STATE XQUE XSTA XTRN XUSR * X-ANONYMOUSTLS CHUNKING X-ADAT X-DRCP
                           X-ERCP X-EXCH50
         b64_decode_depth: -1 (unlimited)
          qp_decode_depth: -1 (unlimited)
          uu_decode_depth: -1 (unlimited)
      bitenc_decode_depth: -1 (unlimited)
              ignore_data: disabled
           decompress_pdf: disabled
           decompress_swf: disabled
           decompress_zip: disabled
           decompress_vba: disabled







           ┌──(kali㉿kali)-[~]
└─$ find /etc -name snort.lua 2>/dev/null        
/etc/snort/snort.lua
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo nano /etc/snort/snort.lua            
[sudo] password for kali: 
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo snort -c /etc/snort/snort.lua -T
[sudo] password for kali: 
--------------------------------------------------
o")~   Snort++ 3.12.2.0
--------------------------------------------------
Loading /etc/snort/snort.lua:
Loading snort_defaults.lua:
Finished snort_defaults.lua:
        active
        alerts
        daq
        decode
        host_cache
        host_tracker
        hosts
        network
        packets
        process
        search_engine
        ips
        stream
        stream_ip
        stream_icmp
        stream_tcp
        stream_udp
        stream_user
        stream_file
        arp_spoof
        back_orifice
        dns
        imap
        netflow
        pop
        rpc_decode
        sip
        socks
        ssh
        ssl
        telnet
        cip
        dnp3
        iec104
        modbus
        dce_smb
        dce_tcp
        dce_udp
        dce_http_proxy
        dce_http_server
        gtp_inspect
        port_scan
        smtp
        ftp_server
        ftp_client
        ftp_data
        http_inspect
        http2_inspect
        classifications
        references
        file_policy
        js_norm
        appid
        wizard
        binder
        file_inspect
        s7commplus
        opcua
        mms
        normalizer
        output
Finished /etc/snort/snort.lua:
Loading file_inspect.rules_file:
Loading file_magic.rules:
Finished file_magic.rules:
Finished file_inspect.rules_file:
--------------------------------------------------
ips policies rule stats
              id  loaded  shared enabled    file
               1     219       0     219    /etc/snort/snort.lua
--------------------------------------------------
rule counts
       total rules loaded: 219
               text rules: 219
            option chains: 219
            chain headers: 1
--------------------------------------------------
service rule counts          to-srv  to-cli
                  file_id:      219     219
                    total:      219     219
--------------------------------------------------
fast pattern groups
                to_server: 1
                to_client: 1
--------------------------------------------------
search engine (ac_bnfa)
appid: MaxRss diff: 2688
appid: patterns loaded: 300
--------------------------------------------------
pcap DAQ configured to passive.

Snort successfully validated the configuration (with 0 warnings).
o")~   Snort exiting





┌──(kali㉿kali)-[~/snort_src/snort3/build]
└─$ ls -l ~/snort_src/snort3
total 516
drwxrwxr-x  8 kali kali   4096 Jul 22 15:34 build
-rw-rw-r--  1 kali kali 311822 Jul 22 13:09 ChangeLog.md
drwxrwxr-x  2 kali kali   4096 Jul 22 13:09 cmake
-rw-rw-r--  1 kali kali   5368 Jul 22 13:09 CMakeLists.txt
-rw-rw-r--  1 kali kali   1034 Jul 22 13:09 cmake_uninstall.cmake.in
-rw-rw-r--  1 kali kali   4884 Jul 22 13:09 config.cmake.h.in
-rwxrwxr-x  1 kali kali  23008 Jul 22 13:09 configure_cmake.sh
-rw-rw-r--  1 kali kali  21011 Jul 22 13:09 COPYING
-rw-rw-r--  1 kali kali  70959 Jul 22 13:09 crusty.cfg
drwxrwxr-x  2 kali kali   4096 Jul 22 13:09 daqs
drwxrwxr-x  6 kali kali   4096 Jul 22 13:09 doc
-rw-rw-r--  1 kali kali  21017 Jul 22 13:09 LICENSE
drwxrwxr-x  2 kali kali   4096 Jul 22 13:09 lua
-rw-rw-r--  1 kali kali   8767 Jul 22 13:09 README.md
-rw-rw-r--  1 kali kali    939 Jul 22 13:09 snort.pc.in
drwxrwxr-x 49 kali kali   4096 Jul 22 13:09 src
drwxrwxr-x  6 kali kali   4096 Jul 22 13:09 tools

