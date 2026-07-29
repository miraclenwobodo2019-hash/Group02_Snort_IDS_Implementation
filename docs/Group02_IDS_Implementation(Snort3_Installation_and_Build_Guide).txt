Snort 3 Installation and Build Guide (Detailed)

This guide expands every step and includes: - Explanation of every
command - Screenshot placeholders - Expected terminal output - Common
errors and fixes encountered during installation

1. Update Kali Linux

Command:

    sudo apt update
    sudo apt upgrade -y

Explanation: - apt update refreshes package indexes. - apt upgrade -y
installs the latest package versions.

Screenshot Placeholder: Insert terminal showing update completed.

Expected Output: Package lists read successfully with upgraded packages.

2. Install Dependencies

    sudo apt install -y build-essential cmake git pkg-config libpcap-dev libpcre2-dev libdumbnet-dev zlib1g-dev liblzma-dev libluajit-5.1-dev libssl-dev libhwloc-dev libunwind-dev bison flex autotools-dev libfl-dev libcmocka-dev libnetfilter-queue-dev libmnl-dev libtirpc-dev uuid-dev

Explanation: - Installs compiler, CMake, Git and all libraries required
to compile Snort.

Screenshot Placeholder: Dependencies installation.

Expected Output: Packages installed successfully.

3. Install DAQ

    sudo apt install -y libdaq-dev
    pkg-config --modversion libdaq

Explanation: DAQ provides packet acquisition support.

Common issue: - pkg-config cannot find libdaq. Fix:

    sudo apt install libdaq-dev

4. Download Snort Source

    git clone --depth=1 https://github.com/snort3/snort3.git
    cd snort3

Explanation: Downloads the latest Snort 3 source.

5. Configure Build

    cmake .

If DAQ is not detected:

    cmake -DDAQ_INCLUDE_DIR=/usr/include -DDAQ_LIBRARY=/usr/lib/x86_64-linux-gnu/libdaq.so .

Common issue encountered: CMake failed because DAQ headers/libraries
were not found. Solution: Specify the DAQ include and library paths
explicitly.

6. Build

    make -j$(nproc)

Explanation: Compiles Snort using all available CPU cores.

Expected output: Compilation reaches 100%.

7. Install

    sudo make install
    sudo ldconfig
    snort -V

Expected: Snort++ version information is displayed.

8. Configure Snort

Create directories:

    sudo mkdir -p /usr/local/etc/snort
    sudo mkdir -p /usr/local/etc/rules
    sudo mkdir -p /var/log/snort

Copy Lua files and create local rules.

Edit snort.lua: - Set HOME_NET. - Keep EXTERNAL_NET as any. - Include
local.rules.

9. Validate

    sudo snort -T -c /usr/local/etc/snort/snort.lua

Expected: Configuration validated successfully.

10. Run

    ip addr
    sudo snort -i eth0 -A alert_fast -c /usr/local/etc/snort/snort.lua

Replace eth0 if another interface is used.

Common Errors We Resolved

1.  DAQ detection failure during CMake.
2.  Incorrect monitoring interface.
3.  Missing include for local.rules.
4.  HOME_NET mismatch.
5.  Rules not triggering until configuration was corrected.

Final Verification Checklist

-   Snort version displays.
-   Configuration test passes.
-   Correct interface selected.
-   Live alerts generated.
