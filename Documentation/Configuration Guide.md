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
