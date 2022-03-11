Change log
-----------

# v2.95.1
## (2022-03-11)


<details>
<summary> Update layers/meta-balena to 9191bc412d404e761d672d1750cd7fe5e2418550 [Renovate Bot] </summary>

> ## meta-balena-2.95.1
> ### (2022-03-08)
> 
> * tests: Add leviathan v2.0.0 as a submodule [Kyle Harding]
> * tests/cloud: Cleanup wait until loops in cloud suite [Kyle Harding]
> * tests/hup: Remove bluebird and this.context.get references [Kyle Harding]
> * tests/os: Remove bluebird and this.context.get references [Kyle Harding]
> * tests/cloud: Remove bluebird and this.context.get references [Kyle Harding]
> * tests: Cleanup suites config to support both testbot and qemu workers [Kyle Harding]
> * tests/cloud: Update cloud suite to support core on client [Kyle Harding]
> * tests/hup: Update hup suite to support core on client [Kyle Harding]
> * tests/os: Update os suite to support core on client [Kyle Harding]
> 
> ## meta-balena-2.95.0
> ### (2022-03-04)
> 
> * Adds modem test suite [Alex]
> 
> ## meta-balena-2.94.5
> ### (2022-03-04)
> 
> * Use by-state symlink for mounting the EFI partition when split [Michal Toman]
> * os-helpers: add TPM2 helpers [Michal Toman]
> * Add PCR protection policy to TPM operation unlocking LUKS passphrase [Michal Toman]
> 
> ## meta-balena-2.94.4
> ### (2022-03-04)
> 
> * balena-supervisor: Fix supervisor tagging command [Florin Sarbu]
> 
> ## meta-balena-2.94.3
> ### (2022-03-02)
> 
> * tests/os: fix bracket in bbb overlay test [rcooke-warwick]
> 
> ## meta-balena-2.94.2
> ### (2022-03-02)
> 
> * tests: Enhance BeagleBone Black u-boot overlay test [Florin Sarbu]
> 
> ## meta-balena-2.94.1
> ### (2022-03-01)
> 
> * balena-image: Default image type to balenaos-img [Alex Gonzalez]
> * Remove legacy resinhup images. [Alex Gonzalez]
> 
> ## meta-balena-2.94.0
> ### (2022-03-01)
> 
> 
> <details>
> <summary> Update balena-supervisor to v12.11.36 [Robert Günzler] </summary>
> 
>> ### balena-supervisor-12.11.36
>> #### (2022-02-23)
>> 
>> * Ignore selinux security opts when comparing services [Felipe Lalanne]
>> 
>> ### balena-supervisor-12.11.35
>> #### (2022-02-16)
>> 
>> * Add troubleshooting notice for macOS [fisehara]
>> 
>> ### balena-supervisor-12.11.34
>> #### (2022-02-15)
>> 
>> * Create `touch` and `getBootTime` utility functions [Felipe Lalanne]
>> * Add update lock check to PATCH /v1/device/host-config [Christina Wang]
>> 
>> ### balena-supervisor-12.11.33
>> #### (2022-02-09)
>> 
>> * Add support for local ipv6 reporting [Felipe Lalanne]
>> 
> </details>
> 
> * meta-resin-pyro: make sure $GO is set [Robert Günzler]
> * Refactor balena-engine recipe to more closely resemble upstream [Robert Günzler]
> * Update Golang recipes to 1.16.2 [Robert Günzler]
> 
> <details>
> <summary> Update balena-engine to v20.10.12 [Robert Günzler] </summary>
> 
>> ### balena-engine-20.10.12
>> #### (2022-02-18)
>> 
>> * storagemigration: keep going if migration fails [Robert Günzler]
>> * graphdriver/copy: fix handling of sockets [Robert Günzler]
>> * pkg/storagemigration: use graphdriver/copy.DirCopy [Robert Günzler]
>> * Prune Jenkinsfile [Robert Günzler]
>> * Backport platform-detection fixes from containerd [Robert Günzler]
>> * storagemigration: capture failcleanup logs in logfile [Robert Günzler]
>> * storagemigration: move logic to package [Robert Günzler]
>> * prevent slice oob access in concatReadSeekCloser [Martin Rauscher]
>> * Make layer download resuming more resilient [Leandro Motta Barros]
>> * Drop CODEOWNERS [Robert Günzler]
>> * pkg/storagemigration: poperly handle errors during state creation [Robert Günzler]
>> * pkg/storagemigration: allow writing logs to separate file [Robert Günzler]
>> * storagemigration: defer commit to next start [Robert Günzler]
>> * Lock destination layers while delta is being processed [Robert Günzler]
>> * Add aufs to overlay2 migrator [Robert Günzler]
>> * Update the README [Robert Günzler]
>> * Cleanup repo [Robert Günzler]
>> * Add a SECURITY.md [Robert Günzler]
>> * top_unix.go: allow busybox ps with no args [Kyle Harding]
>> * Bump balena-os/balena-containerd to 1da48a8 [Tian Yuanhao]
>> * Add changelog template to allow generating nested changelogs [Robert Günzler]
>> * Update github issue and pr templates [Robert Günzler]
>> * Update codeowners [Robert Günzler]
>> * hack: Fix CLI versioning [Robert Günzler]
>> * Fixed typos in getting-started.md docs [Miguel Casqueira]
>> * Add integration tests for hostapp handling [Robert Günzler]
>> * Fix container data deletion [Roman Mazur]
>> * overlay2: Add List support [Roman Mazur]
>> * aufs: Add List support [Roman Mazur]
>> * layer: Remove unreferenced driver layers on create [Roman Mazur]
>> * layer: Prune unused data on layer store creation [Roman Mazur]
>> * layer: Persist cacheID early on transaction start [Roman Mazur]
>> * pkg/authorization: Fix test failures on macOS [Roman Mazur]
>> * Move ci to balenaCI [Robert Günzler]
>> * contrib: Add balena-engine version of dind container [Robert Günzler]
>> * build.sh: Disable btrfs,zfs,devicemapper graphdrivers [Robert Günzler]
>> * Bump CLI dependency to include fix for #178 [Robert Günzler]
>> * Bump CLI dependency to include --cidenv flag [Robert Günzler]
>> * Allow passing container ID to container via environment variable [Robert Günzler]
>> * contrib/install.sh: Add details to the success message [Robert Günzler]
>> * contrib/install.sh: Rename balena to balenaEngine in ASCII art output [Robert Günzler]
>> * contrib/install.sh: Fail on error [Robert Günzler]
>> * Add daemon flags to configure max download/upload attempts during pull/push [Robert Günzler]
>> * aufs,overlay2: Add driver opts for disk sync [Robert Günzler]
>> * Fix double locking in the event handling code of OOM events [Robert Günzler]
>> * integration-tests: Add test for containers with memory,cpu constraints [Robert Günzler]
>> * Update Dockerfiles used for build to Go 1.10.8 [Robert Günzler]
>> * travis: Use the minimal machine [Robert Günzler]
>> * Add cli for tagging delta images [Robert Günzler]
>> * Allow tagging of image deltas on creation [Robert Günzler]
>> * docs: Fix Docker capitalisation in balenaEngine docs [Paulo Castro]
>> * Update balenaEngine logo in README.md [Paulo Castro]
>> * Disable incompatible integration tests [Paulo Castro]
>> 
>> ### balena-engine-20.10.11
>> #### (2021-12-09)
>> 
>> * Merge upstream v20.10.11 [Robert Günzler]
>> 
> </details>
> 
> 
> ## meta-balena-2.93.2
> ### (2022-03-01)
> 
> * prepare-openvpn: Make configurable [Alex Gonzalez]
> 
> ## meta-balena-2.93.1
> ### (2022-02-28)
> 
> * tests/cloud: Use deviceID returned from pre-registration [Kyle Harding]
> 
> ## meta-balena-2.93.0
> ### (2022-02-26)
> 
> * resin-device-register: Use supervisor version label instead of tag [Alex Gonzalez]
> * balena-supervisor: Rename repository/tag to fleet/version [Alex Gonzalez]
> * docker-disk: entry.sh: Rename repository/tag to fleet/version [Alex Gonzalez]
> 
> ## meta-balena-2.92.0
> ### (2022-02-25)
> 
> * Update ModemManager to v1.18.4 [Zahari Petkov]
> 
> ## meta-balena-2.91.6
> ### (2022-02-25)
> 
> * resin-device-register: Regenerate VPN credentials on registration [Alex Gonzalez]
> * resin-init-flasher: Wait for resin-device-register to start [Alex Gonzalez]
> 
> ## meta-balena-2.91.5
> ### (2022-02-24)
> 
> * suites/os: Add testcase for RPi device-tree [Alexandru Costache]
> 
> ## meta-balena-2.91.4
> ### (2022-02-24)
> 
> * openvpn: Remove dependency on timesync-http target [Alex Gonzalez]
> 
> ## meta-balena-2.91.3
> ### (2022-02-24)
> 
> * tests/os: Wait for os-config-json service to be inactive [Kyle Harding]
> 
> ## meta-balena-2.91.2
> ### (2022-02-23)
> 
> * contributing-device-support.md: Updates to board support instructions [Florin Sarbu]
> 
> ## meta-balena-2.91.1
> ### (2022-02-21)
> 
> * tests/cloud: wait for update lock message in logs [rcooke-warwick]
> * tests/cloud: register teardown before  online [rcooke-warwick]
> 
> ## meta-balena-2.91.0
> ### (2022-02-14)
> 
> * openssh: Add a dependency on os-sshkeys [Alex Gonzalez]
> * balena-supervisor: Add dependency on root CA [Alex Gonzalez]
> * balena: Add dependency on balena-hostname [Alex Gonzalez]
> * Make services configurable [Alex Gonzalez]
> * classes: Add balena-configurable [Alex Gonzalez]
> * balena-config-vars: Split config.json configuration on write [Alex Gonzalez]
> * Remove config-json.target [Alex Gonzalez]
> 
> ## meta-balena-2.90.0
> ### (2022-02-13)
> 
> * resin-init-flasher: check for UEFI mode and set config variables [Mark Corbin]
> * resin-init-flasher: Fix flashing progress reporting for LUKS [Michal Toman]
> * resin-init-flasher: Use flasher kernel to emulate stage2 bootloader with LUKS [Michal Toman]
> * resin-init-flasher: Add support for opt-in full disk encryption [Michal Toman]
> 
> ## meta-balena-2.89.19
> ### (2022-02-13)
> 
> * README: Update versioning information [Alex Gonzalez]
> 
> ## meta-balena-2.89.18
> ### (2022-02-11)
> 
> * fix cloud suite teardown [rcooke-warwick]
> 
> ## meta-balena-2.89.17
> ### (2022-02-09)
> 
> * suites/hup: Add under-voltage test before and after HUP [Alexandru Costache]
> 
> ## meta-balena-2.89.16
> ### (2022-02-07)
> 
> * balena-supervisor: Update balena-supervisor to v12.11.32 [Felipe Lalanne]
> 
> ## meta-balena-2.89.15
> ### (2022-02-07)
> 
> * resindataexpander: do not return after resizing the partition only [Michal Toman]
> 
> ## meta-balena-2.89.14
> ### (2022-02-03)
> 
> * resin-u-boot.bbclass: Do not error if no config_defaults.h [Florin Sarbu]
> 
> ## meta-balena-2.89.13
> ### (2022-02-01)
> 
> * docker-disk: Tag the supervisor digest with the repo name [Kyle Harding]
> 
> ## meta-balena-2.89.12
> ### (2022-02-01)
> 
> * resindataexpander: expand fs independent of partition [Joseph Kogut]
> 
> ## meta-balena-2.89.11
> ### (2022-01-29)
> 
> * image_types_balena: Augment dependency on u-boot do_deploy task [Florin Sarbu]
> 
> ## meta-balena-2.89.10
> ### (2022-01-28)
> 
> * tests: relax boot splash screen check [rcooke-warwick]
> 
> ## meta-balena-2.89.9
> ### (2022-01-27)
> 
> * archive logs using local ssh [rcooke-warwick]
> * put archiver in the right place [rcooke-warwick]
> * Enable UART serial console for supported devices [Kyle Harding]
> * archive image on teardown [rcooke-warwick]
> * put device in dev mode [rcooke-warwick]
> * tests: add extra logging to cloud suite [rcooke-warwick]
> 
> ## meta-balena-2.89.8
> ### (2022-01-27)
> 
> * u-boot: Move config fragments merging code out of common layer [Florin Sarbu]
> 
> ## meta-balena-2.89.7
> ### (2022-01-26)
> 
> * explain balenaRootCA better [Martin Rauscher]
> 
> ## meta-balena-2.89.6
> ### (2022-01-26)
> 
> * classes/kernel-balena: Update aufs patches for kernel 5.10.82 [Alexandru Costache]
> 
> ## meta-balena-2.89.5
> ### (2022-01-24)
> 
> * os: tests: optimize fingerprint tests [Joseph Kogut]
> 
> ## meta-balena-2.89.4
> ### (2022-01-21)
> 
> * tests: add cloud test suite [rcooke-warwick]
> 
> ## meta-balena-2.89.3
> ### (2022-01-20)
> 
> * initramfs-framework: Make cleaning udev database the last step [Alex Gonzalez]
> 
> ## meta-balena-2.89.2
> ### (2022-01-20)
> 
> * recipes-core/jq: Use 64bit time symbols [Alexandru Costache]
> 
> ## meta-balena-2.89.1
> ### (2022-01-19)
> 
> * tests: Enable UART serial console where supported [Kyle Harding]
> 
> ## meta-balena-2.89.0
> ### (2022-01-19)
> 
> * docker-disk: Pull images from Balena's registry [Alex Gonzalez]
> * balena-supervisor: Use image location path instead of repository:tag [Alex Gonzalez]
> * distro: balena-os: Add default cloud environment distro setting [Alex Gonzalez]
> 
> ## meta-balena-2.88.22
> ### (2022-01-18)
> 
> * intel-quark: Fix to honister syntax [Alex Gonzalez]
> * recipes-core/bash: Use 64bit time symbols [Alexandru Costache]
> * recipes-core/busybox: Use 64bit time symbols [Alexandru Costache]
> 
> ## meta-balena-2.88.21
> ### (2022-01-17)
> 
> * tests: os: config-json: cleanup persistentLogging test [Joseph Kogut]
> * tests: os: config-json: return promise from sshKeys test [Joseph Kogut]
> * tests: os: config-json: cleanup dnsServers config test [Joseph Kogut]
> * tests: os: config-json: cleanup ntpServer config test [Joseph Kogut]
> * tests: os: config-json: cleanup hostname config test [Joseph Kogut]
> * tests: os: create waitForServiceState helper [Joseph Kogut]
> * tests: os: config-json: remove reboot from randomMacAddressScan test [Joseph Kogut]
> * tests: os: config-json: remove reboot from connectivity test [Joseph Kogut]
> * tests: os: config-json: remove reboot from udevRules test [Joseph Kogut]
> 
> ## meta-balena-2.88.20
> ### (2022-01-17)
> 
> * chrony: fix mount service dependency for driftfile [Mark Corbin]
> 
> ## meta-balena-2.88.19
> ### (2022-01-12)
> 
> * os: tests: optimize fsck tests [Joseph Kogut]
> 
> ## meta-balena-2.88.18
> ### (2022-01-11)
> 
> * conf/distro: Prefer rust v1.36 for releases older than Honister [Alexandru Costache]
> 
> ## meta-balena-2.88.17
> ### (2022-01-10)
> 
> * recipes-core/coreutils: Use 64bit time symbols [Alexandru Costache]
> * classes/image_types_balena: Preserve file modification times with mcopy [Alexandru Costache]
> 
> ## meta-balena-2.88.16
> ### (2022-01-05)
> 
> * balena-os.inc: Switch balena backend storage to overlay2 [Florin Sarbu]
> 
> ## meta-balena-2.88.15
> ### (2022-01-04)
> 
> * initrdscripts: fsuuidinit: Generate resin-rootA last [Alex Gonzalez]
> * lvm2: Add rule to persist dm devices in udev database [Alex Gonzalez]
> * initrdscript: Cleanup udev database before transitioning to rootfs [Alex Gonzalez]
> * initrdscripts: Use /run as bootparam_root storage [Alex Gonzalez]
> * lvm: Add lvm rules when secure boot is configured [Alex Gonzalez]
> * balena-keys: Fetch DER keys and decode from base64 [Alex Gonzalez]
> 
> ## meta-balena-2.88.14
> ### (2022-01-04)
> 
> * Sync cached writes to disk when updating supervisor.conf [Miguel Casqueira]
> 
> ## meta-balena-2.88.13
> ### (2022-01-04)
> 
> * hostapp-update-hooks: Handle developmentMode updates [Alex Gonzalez]
> 
> ## meta-balena-2.88.12
> ### (2022-01-03)
> 
> * systemd/timeinit: handle missing date field in HTTPS header [Mark Corbin]
> 
> ## meta-balena-2.88.11
> ### (2021-12-22)
> 
> * balena-supervisor: Update balena-supervisor to v12.11.16 Update balena-supervisor from 12.11.0 to 12.11.16 [Miguel Casqueira]
> 
> ## meta-balena-2.88.10
> ### (2021-12-16)
> 
> * Update NetworkManager to 1.32.12 [Zahari Petkov]
> 
> ## meta-balena-2.88.9
> ### (2021-12-15)
> 
> * u-boot: Move u-boot configs inclusion into resin-u-boot.bbclass [Florin Sarbu]
> 
> ## meta-balena-2.88.8
> ### (2021-12-09)
> 
> * patch: Add archiveLogs Teardown for HUP suite [Vipul Gupta]
> 
> ## meta-balena-2.88.7
> ### (2021-12-06)
> 
> * tests: Ensure BDADDR is initialized [Alexandru Costache]
> 
> ## meta-balena-2.88.6
> ### (2021-12-04)
> 
> * docs: Fix links in Rollback documentation [Kyle Harding]
> 
> ## meta-balena-2.88.5
> ### (2021-12-04)
> 
> * tests: os: fix unhandled exception when unwrapping non-flasher image [Joseph Kogut]
> 
> ## meta-balena-2.88.4
> ### (2021-12-03)
> 
> * tests: Add basic checks for data loss during HUP [Kyle Harding]
> * hostapp-update-hooks: Ensure data breadcrumb is present before HUP [Kyle Harding]
> 
> ## meta-balena-2.88.3
> ### (2021-12-02)
> 
> * grub-conf: Delay grub boot in os development mode [Alex Gonzalez]
> * grub-efi: Allow input/output in OS development mode [Alex Gonzalez]
> 
> ## meta-balena-2.88.2
> ### (2021-12-02)
> 
> * sign-efi.bbclass: Do not deploy the unused .signed symlink [Michal Toman]
> * sign-gpg.bbclass: Only deploy the detached signature [Michal Toman]
> * kernel-image-initramfs.bb: Ship kernel and matching signature [Michal Toman]
> * Make kexec work under kernel lockdown [Michal Toman]
> 
> ## meta-balena-2.88.1
> ### (2021-12-02)
> 
> * bluez5: Update to bluez 5.61 from poky honister [Kyle Harding]
> 
> ## meta-balena-2.88.0
> ### (2021-12-01)
> 
> * systemd/timeinit: add HTTPS time synchronisation service [Mark Corbin]
> 
> ## meta-balena-2.87.32
> ### (2021-12-01)
> 
> * tests: Add BeagleBone Black u-boot overlay test [Florin Sarbu]
> 
> ## meta-balena-2.87.31
> ### (Invalid date)
> 
> * resin-update-state.rules: do not run for unnamed partitions [Michal Toman]
> * resin_update_state_probe: do not skip device mapper devices [Michal Toman]
> 
> ## meta-balena-2.87.30
> ### (Invalid date)
> 
> * tests: Add device specific RevPi Core 3 DIO module test [Alexandru Costache]
> 
> ## meta-balena-2.87.29
> ### (2021-11-29)
> 
> * common: image-balena: enable developmentMode when OS_DEVELOPMENT=1 [Joseph Kogut]
> 
> ## meta-balena-2.87.28
> ### (2021-11-26)
> 
> * Add secure boot keys to the flasher boot partition [Alex Gonzalez]
> 
> ## meta-balena-2.87.27
> ### (2021-11-25)
> 
> * balena-os: make sure PAM support is not configured [Alex Gonzalez]
> 
> ## meta-balena-2.87.26
> ### (2021-11-25)
> 
> * tests: add test for filesystem checks [Joseph Kogut]
> * common: initrdscript: fsck resin-data on boot [Joseph Kogut]
> 
> ## meta-balena-2.87.25
> ### (2021-11-25)
> 
> * connectivity: reduce ping interval to minimum [Joseph Kogut]
> 
> ## meta-balena-2.87.24
> ### (2021-11-24)
> 
> * tests: Fix dnsmasq tests in cases where 8.8.8.8 is assigned via DHCP [Kyle Harding]
> 
> ## meta-balena-2.87.23
> ### (2021-11-24)
> 
> * 0-signed-update HUP hook: mount efivarfs if necessary [Michal Toman]
> 
> ## meta-balena-2.87.22
> ### (2021-11-24)
> 
> * grub-efi: Accept no input and output nothing when in secure boot mode [Michal Toman]
> 
> ## meta-balena-2.87.21
> ### (2021-11-24)
> 
> * linux-firmware: Include MT7601U firmware [Zahari Petkov]
> 
> ## meta-balena-2.87.20
> ### (2021-11-23)
> 
> * balena-image: Add balena keys to boot partition if required [Alex Gonzalez]
> * grub-conf: Enforce module signing and integrity lockdown on luks config [Alex Gonzalez]
> * distro: balena-os: Add empty SIGN_API [Alex Gonzalez]
> * classes: image-balena: Copy signed files if present [Alex Gonzalez]
> * classes/sign-gpg: Rename class to sign_gpg [Alex Gonzalez]
> * classes: Rename sign to sign-gpg [Alex Gonzalez]
> * classes: sign: Drop suffix from deployed files [Alex Gonzalez]
> * resin-init-flasher: Set fde grub.cfg if secure boot is enabled [Alex Gonzalez]
> * balena-image-initramfs: Add secure boot dependencies [Alex Gonzalez]
> * kernel-image-initramfs: Install signed kernel images if available [Alex Gonzalez]
> * kernel-balena: Configure for secure boot [Alex Gonzalez]
> 
> ## meta-balena-2.87.19
> ### (2021-11-22)
> 
> * common: enable multi-label mDNS resolution and IPv6 [Joseph Kogut]
> 
> ## meta-balena-2.87.18
> ### (2021-11-22)
> 
> * unwrap flasher images in os suite if needed [rcooke-warwick]
> * bluetooth and hup test with qemu [rcooke-warwick]
> 
> ## meta-balena-2.87.17
> ### (2021-11-21)
> 
> * efitools: Add recipe [Alex Gonzalez]
> * sbsigntool: Add recipe [Alex Gonzalez]
> 
> ## meta-balena-2.87.16
> ### (2021-11-21)
> 
> * peak: Modify kernel driver to use signing class [Alex Gonzalez]
> 
> ## meta-balena-2.87.15
> ### (2021-11-21)
> 
> * kernel-balena.class: Add support for FDE and sign for secure boot [Michal Toman]
> 
> ## meta-balena-2.87.14
> ### (2021-11-21)
> 
> * sign-efi.bbclass: do not mix old and new bitbake syntax [Michal Toman]
> * Revert "sign-efi.class, sign-kmod.class: Replace original files with signed ones" [Michal Toman]
> 
> ## meta-balena-2.87.13
> ### (2021-11-20)
> 
> * meta-resin-sumo/pyro: Fix initramfs-framework kexec dependencies [Alex Gonzalez]
> * initrdscripts: Use a 2nd stage bootloader to unlock LUKS partitions [Michal Toman]
> * grub-efi: add support for signature verification in secure boot mode [Michal Toman]
> 
> ## meta-balena-2.87.12
> ### (2021-11-20)
> 
> * initramfs-module-cryptsetup: add TPM dependencies [Michal Toman]
> 
> ## meta-balena-2.87.11
> ### (2021-11-20)
> 
> * balena-keys: Add recipe [Alex Gonzalez]
> 
> ## meta-balena-2.87.10
> ### (2021-11-20)
> 
> * sign-efi.class, sign-kmod.class: Replace original files with signed ones [Michal Toman]
> * Add signing classes [Alex Gonzalez]
> 
> ## meta-balena-2.87.9
> ### (2021-11-17)
> 
> * hostapp-update-hooks: Add a hook that aborts HUP to unsigned OS under secure boot [Michal Toman]
> 
> ## meta-balena-2.87.8
> ### (2021-11-17)
> 
> * resin-mounts: mount EFI partition if it is split from boot [Michal Toman]
> 
> ## meta-balena-2.87.7
> ### (2021-11-16)
> 
> * initrdscripts: add a script for unlocking LUKS volumes [Michal Toman]
> 
> ## meta-balena-2.87.6
> ### (2021-11-15)
> 
> * connectivity: proxy: move nadoo/glider to container [Joseph Kogut]
> 
> ## meta-balena-2.87.5
> ### (2021-11-11)
> 
> * tests: os: Add exposed engine socket test [Alex Gonzalez]
> 
> ## meta-balena-2.87.4
> ### (2021-11-11)
> 
> * resindataexpander: also resize LUKS volume if necessary [Michal Toman]
> 
> ## meta-balena-2.87.3
> ### (2021-11-11)
> 
> * Add out-of-tree peak CAN driver [Michal Toman]
> 
> ## meta-balena-2.87.2
> ### (2021-11-11)
> 
> * Add recipes for TPM2 tools [Michal Toman]
> 
> ## meta-balena-2.87.1
> ### (2021-11-10)
> 
> * recipes-devtools/dosfstools: Fix build with Poky Honister [Alexandru Costache]
> 
> ## meta-balena-2.87.0
> ### (2021-11-09)
> 
> * meta-balena-common/conf: Switch layer to Honister compatibility [Alexandru Costache]
> 
> ## meta-balena-2.86.3
> ### (2021-11-09)
> 
> * patch: Fix URL to yocto project dependencies [Kyle Harding]
> 
> ## meta-balena-2.86.2
> ### (2021-11-08)
> 
> * dosfstools: selectively apply upstreamed patch [Joseph Kogut]
> * tests: wait for the chronyd service become active [Mark Corbin]
> 
> ## meta-balena-2.86.1
> ### (2021-11-02)
> 
> * tests/issue: Add test to check issues files [Alex Gonzalez]
> * base files: Use HOSTOS_VERSION in issue and issue.net [Alex Gonzalez]
> 
> ## meta-balena-2.86.0
> ### (2021-10-29)
> 
> * Create new data partition reset service [Kyle Harding]
> 
> ## meta-balena-2.85.17
> ### (2021-10-28)
> 
> * restrict dtoverlay test to rpi devices [rcooke-warwick]
> 
</details>

* Update balena-yocto-scripts to c4783384e08d29a53905290ef9f44b45c4a756a2 [Renovate Bot]
* Add renovate configuration [Alex Gonzalez]
* Add versionist workflow [Alex Gonzalez]
* Add test-submodules [Alex Gonzalez]
* Remove renovate configuration [Alex Gonzalez]
* Add renovate configuration [Alex Gonzalez]
* Remove configuration to force onboarding [Alex Gonzalez]
* Update renovate configuration [Alex Gonzalez]
* Unconfigure renovate [Alex Gonzalez]
* Disable renovate automerge [Alex Gonzalez]

# v2.85.16+rev10
## (2022-03-03)

* Configure renovatebot for nested changelog support [Alex Gonzalez]

# v2.85.16+rev9
## (2022-02-28)

* Remove versionist package.json [Alex Gonzalez]

# v2.85.16+rev8
## (2022-02-26)


<details>
<summary> Update balena-yocto-scripts to v1.17.2 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.17.2
> ### (2022-02-25)
> 
> * prepare-and-start: Remove balena login [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.17.1
> ### (2022-01-27)
> 
> * balena-deploy.inc: Do no deploy device logo to deprecated endpoint [Florin Sarbu]
> 
</details>

# v2.85.16+rev7
## (2022-01-21)


<details>
<summary> Update balena-yocto-scripts to v1.17.0 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.17.0
> ### (2022-01-20)
> 
> * balena-lib: Fix fetching meta-balena base version [Alex Gonzalez]
> * jenkins_build-block: Use true/false for ESR variable [Alex Gonzalez]
> * balena-deploy-block: Label ESR hostapps [Alex Gonzalez]
> * balena-api: add balena_api_fetch_fleet_tag [Alex Gonzalez]
> * balena-api: Set policy on ESR hostapps [Alex Gonzalez]
> * balena-deploy: Pass ESR variable when creating apps [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.16.4
> ### (2022-01-18)
> 
> * balena-deploy: Deploy passing the latest meta-balena version and not tag [Alex Gonzalez]
> * balena-lib: Add balena_lib_get_meta_balena_base_version [Alex Gonzalez]
> 
</details>

# v2.85.16+rev6
## (2022-01-18)


<details>
<summary> Update balena-yocto-scripts to v1.16.3 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.16.3
> ### (2022-01-17)
> 
> * balena-deploy-block: Check for existing tag only in specific hostapp [Alex Gonzalez]
> 
</details>

# v2.85.16+rev5
## (2022-01-15)


<details>
<summary> Update balena-yocto-scripts to v1.16.2 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.16.2
> ### (2022-01-15)
> 
> * balena-api: Propagate balena API environment, token and OS organization [Alex Gonzalez]
> * balena-build.sh: Propagate balena API environment and token [Alex Gonzalez]
> * prepare-and-start: Propagate balena API environment and token [Alex Gonzalez]
> 
</details>

# v2.85.16+rev4
## (2022-01-14)


<details>
<summary> Update balena-yocto-scripts to v1.16.1 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.16.1
> ### (2022-01-11)
> 
> * revert_overrides: Add intel-quark to architecture overrides [Alex Gonzalez]
> 
</details>

# v2.85.16+rev3
## (2021-12-30)


<details>
<summary> Update balena-yocto-scripts to v1.16.0 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.16.0
> ### (2021-12-30)
> 
> * balena-deploy: Check for file existence before deploying [Alex Gonzalez]
> * balena-deploy-block: Check existence of tag before re-deploying [Alex Gonzalez]
> * balena-api: Add function to check the existence of a release tag [Alex Gonzalez]
> * balena-deploy-block: Finalize releases when deployed [Alex Gonzalez]
> * Accept deployments without balena.yml [Alex Gonzalez]
> * jenkins_generate_ami: Remove variant from image name [Alex Gonzalez]
> * balena-build.sh: Stop building OS variants [Alex Gonzalez]
> * jenkins_build.sh: Remove buildFlavor [Alex Gonzalez]
> * jenkins_build-blocks: Remove variant build option [Alex Gonzalez]
> * balena-deploy: Stop using .dev/.prod variant suffixes [Alex Gonzalez]
> * balena-deploy-block: Stop tagging hostapp releases with variant [Alex Gonzalez]
> * balena-lib: Use externalVersion to match contracts [Alex Gonzalez]
> * jenkins_build: Deploy hostapp like any other block [Alex Gonzalez]
> * jenkins_build-blocks: Separate block build release deployment [Alex Gonzalez]
> * balena-deploy-block: Use release versioning [Alex Gonzalez]
> * jenkins_build: Remove discontinued check [Alex Gonzalez]
> * balena-deploy: Do not deploy discontinued device types [Alex Gonzalez]
> * balena-deploy: Discontinued device types use meta-balena version [Alex Gonzalez]
> * balena-deploy: Adapt balena_deploy_block to release versioning and use it [Alex Gonzalez]
> * balena-build-block: Remove image release [Alex Gonzalez]
> * balena-api: Use release revision for fetchers [Alex Gonzalez]
> * jenkins_build-block: Remove release version API setter [Alex Gonzalez]
> * balena-api: Remove release version API setter [Alex Gonzalez]
> * balena-lib: Use release versioning [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.15.10
> ### (2021-12-02)
> 
> * balena-deploy: Set leviathan networkWireless mode based on device slug [Kyle Harding]
> 
> ## balena-yocto-scripts-1.15.9
> ### (2021-11-26)
> 
> * Substitute the worker types for generic device slugs [Kyle Harding]
> 
> ## balena-yocto-scripts-1.15.8
> ### (2021-11-03)
> 
> * Dockerfile_yocto-build-env: Install Honister host deps [Alexandru Costache]
> 
> ## balena-yocto-scripts-1.15.7
> ### (2021-10-25)
> 
> * jenkins_build.sh: Fix deployment for discontinued device types [Alex Gonzalez]
> * jenkins_build.sh: Remove PRIVATE_DT as it is unused [Alex Gonzalez]
> * jenkins_build.sh: Fix lint warnings [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.15.6
> ### (2021-10-21)
> 
> * balena-generate-ami.sh: wait for boot partition when preloading AMI [Michal Toman]
> 
> ## balena-yocto-scripts-1.15.5
> ### (2021-10-21)
> 
> * jenkins_generate_ami.sh: Use a shared directory for preloaded image [Michal Toman]
> 
> ## balena-yocto-scripts-1.15.4
> ### (2021-10-20)
> 
> * barys: update development image variables [Mark Corbin]
> 
> ## balena-yocto-scripts-1.15.3
> ### (2021-10-20)
> 
> * jenkins_generate_ami.sh: Preload outside of yocto cache [Michal Toman]
> 
> ## balena-yocto-scripts-1.15.2
> ### (2021-10-01)
> 
> * balena-generate-ami.sh: correctly mount boot partition when injecting SSH key [Michal Toman]
> 
> ## balena-yocto-scripts-1.15.1
> ### (2021-10-01)
> 
> * Update balena-cli to 12.50.1 [Michal Toman]
> 
> ## balena-yocto-scripts-1.15.0
> ### (2021-10-01)
> 
> * jenkins_generate_ami.sh: Use lib function to get arch from config.json [Michal Toman]
> * balena-generate-ami.sh: Look for boot partition by label rather than hardcoding p1 [Michal Toman]
> * balena-generate-ami.sh: Fail if AMI already exists [Michal Toman]
> * balena-generate-ami.sh: sync after writing config.json [Michal Toman]
> * balena-generate-ami.sh: Stick to POSIX-compliant [ instead of [[ [Michal Toman]
> * balena-generate-ami.sh: Remove useless statements [Michal Toman]
> * jenkins_generate_ami.sh: Use architecture as suffix instead of machine name [Michal Toman]
> * jenkins_build.sh: pass MACHINE to jenkins_generate_ami.sh [Michal Toman]
> * AMI automation: Adjust AMI names to be compatible with AWS API [ab77]
> * AMI automation: Correct S3 bucket name and key [ab77]
> * AMI automation: Add a separate container for generaing AMI [Michal Toman]
> * AMI automation: shellcheck and resolve violations [ab77]
> * AMI automation: Use staging env by default [Tomás Tormo]
> * AMI automation: Simplify public ssh addition. Do not use sudo [Tomás Tormo]
> * automation: Generate and publish AMI from the raw balenaOS image [Tomás Tormo]
> 
</details>

# v2.85.16+rev2
## (2021-12-30)

* Remove versionist and balena.yml [Alex Gonzalez]

# v2.85.16+rev1
## (2021-12-02)

* Remove device type name from contract [Alex Gonzalez]

# v2.85.16
## (2021-12-02)

* Update meta-balena from v2.85.15 to v2.85.16 [Alex Gonzalez]

# v2.85.15
## (2021-12-02)

* Update meta-balena from v2.85.14 to v2.85.15 [Alex Gonzalez]

# v2.85.14+rev2
## (2021-12-01)

* Update versionist [Alex Gonzalez]

# v2.85.14+rev1
## (2021-11-16)

* Add name to balena contract [Alex Gonzalez]

# v2.85.14
## (2021-11-16)

* Update meta-balena from v2.85.13 to v2.85.14 [Alex Gonzalez]

# v2.85.13
## (2021-11-16)

* Update meta-balena from v2.85.12 to v2.85.13 [Alex Gonzalez]

# v2.85.12+rev2
## (2021-11-16)

* Update versionist [Alex Gonzalez]

# v2.85.12+rev1
## (2021-11-16)

* Update versionist [Alex Gonzalez]

# v2.85.12
## (2021-11-15)

* Update meta-balena from v2.85.11 to v2.85.12 [Alex Gonzalez]

# v2.85.11+rev2
## (2021-11-15)

* Update versionist [Alex Gonzalez]

# v2.85.11+rev1
## (2021-11-15)

* update versionist to work with ESR [Alex Gonzalez]

# v2.85.11
## (2021-11-12)

* Add a basic contract [Alex Gonzalez]
* Update meta-balena from v2.85.10 to v2.85.11 [Alex Gonzalez]
* Add a local versionist.conf.js [Alex Gonzalez]

# v2.85.10+rev1
## (2021-10-27)

* Update meta-balena from v2.80.1 to v2.85.10 [Alex Gonzalez]

# v2.80.1+rev2
## (2021-09-24)


<details>
<summary> Update balena-yocto-scripts from v1.14.6 to v1.14.9 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.14.9
> ### (2021-08-20)
> 
> * balena-deploy: When deploying hostapp default to using slug as name [Alex Gonzalez]
> * balena-api: Do not use balena_lib_resolve_aliases [Alex Gonzalez]
> * balena_lib: Make resolve_aliases local so it is not globally used [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.14.8
> ### (2021-07-22)
> 
> * Use slug when setting deviceType for leviathan [Kyle Harding]
> 
> ## balena-yocto-scripts-1.14.7
> ### (2021-06-29)
> 
> * balena-lib: Fix print statements helper functions [Kyle Harding]
> * balena-lib: Fix device dir when running in Jenkins containers [Kyle Harding]
> 
</details>

# v2.80.1+rev1
## (2021-06-18)

* Update meta-balena from v2.79.6 to v2.80.1 [Alex Gonzalez]
* Update balena-yocto-scripts from v1.14.3 to v1.14.6 [Alex Gonzalez]

# v2.80.0+rev1
## (2021-06-08)

* Update meta-balena from v2.79.7 to v2.80.0 [Alex Gonzalez]

<details>
<summary> Update balena-yocto-scripts from 1.14.1 to 1.14.3 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.14.3
> ### (2021-06-01)
> 
> * balena-api: Filter out debug output [Alex Gonzalez]
> * balena-api: Specify API environment and token when setting app roles [Alex Gonzalez]
> * jenkins_build-blocks: Separate recipes and packages [Alex Gonzalez]
> * balena-lib: Generalize contract fetcher [Alex Gonzalez]
> * balena-deploy: Shorten installation directory '/yocto/resin-board' to '/work' [Alex Gonzalez]
> * Conditional verbosity mode [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.14.2
> ### (2021-05-26)
> 
> * balena-lib: Add function to fetch labels from image [Alex Gonzalez]
> * balena-lib: contracts: Add package list fetcher [Alex Gonzalez]
> * semver: Add bash utility for semantic version comparison [Alex Gonzalez]
> * balena-docker: Add image retrieval function [Alex Gonzalez]
> 
</details>

* Switch storage driver to overlay2 [Alex Gonzalez]

# v2.79.7+rev1
## (2021-06-08)


<details>
<summary> Update meta-balena from v2.79.4 to v2.79.7 [Mark Corbin] </summary>

> ## meta-balena-2.79.7
> ### (2021-05-26)
> 
> * meta-balena: rename connectivity packagegroup [Mark Corbin]
> 
> ## meta-balena-2.79.6
> ### (2021-05-26)
> 
> * bluez5: Use bluez5 recipe from poky master [Zahari Petkov]
> 
> ## meta-balena-2.79.5
> ### (2021-05-21)
> 
> * README: Update supported Yocto versions [Alex Gonzalez]
> 
</details>

* balena-connectcore: rename connectivity packagegroup [Mark Corbin]

# v2.79.6+rev1
## (2021-06-08)

* Update meta-balena from v2.79.4 to v2.79.6 [Alex Gonzalez]

# v2.79.4+rev1
## (2021-05-24)

* Add balena-yocto-scripts to upstream sources in repo.yml [Alex Gonzalez]
* Update meta-balena from v2.72.1 to v2.79.4 [Alex Gonzalez]

<details>
<summary> Update  balena-yocto-scripts from v1.11.1 to v1.14.1 [Alex Gonzalez] </summary>

> ## balena-yocto-scripts-1.14.1
> ### (2021-05-24)
> 
> * Add a parsable representation of the changelog [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.14.0
> ### (2021-05-21)
> 
> * Dockerfile_yocto-block-build-env: Add container to build Yocto based hostOS blocks [Alex Gonzalez]
> * balena-build-block: Balena build and deploy a hostOS block image [Alex Gonzalez]
> * jenkins_build-blocks: Add package blocks builder script [Alex Gonzalez]
> * balena-deploy: Add functions to deploy block, feed and OS release [Alex Gonzalez]
> * README: Add brief introduction to the main scripts [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.13.0
> ### (2021-05-19)
> 
> * barys: Replace supervisor tag with supervisor release version [Alex Gonzalez]
> * jenkins_build: Replace supervisor tag with supervisor release [Alex Gonzalez]
> * jenkins_build: Rename metaResinBranch to metaBalenaBranch [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.16
> ### (2021-05-18)
> 
> * tests: Substitute deviceType with MACHINE when packaging tests [Kyle Harding]
> 
> ## balena-yocto-scripts-1.12.15
> ### (2021-05-18)
> 
> * Dockerfile_yocto-build-env: Specify docker version [Alex Gonzalez]
> * balena-docker: Allow to control iptables and ipmasq flags [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.14
> ### (2021-05-17)
> 
> * balena-api: Set default argument value not to exist on nounset setting [Alex Gonzalez]
> * balena-api: Allow access to OS developers to public apps [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.13
> ### (2021-05-14)
> 
> * balena-api: Add functions for apps management [Alex Gonzalez]
> * balena-api: Add block images getter functions [Alex Gonzalez]
> * balena-api: Add missing argument to function comments [Alex Gonzalez]
> * balena-deploy-block: Create public app if required [Alex Gonzalez]
> * balena-lib: Fix device installation path when running in helper container [Alex Gonzalez]
> * balena-deploy: Fix device installation path when running in helper container [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.12
> ### (2021-05-12)
> 
> * balena-docker: Adapt to be used from POSIX shell [Alex Gonzalez]
> * balena-docker: Generalize functions to any engine [Alex Gonzalez]
> * balena-build: Re-enable the container's output [Alex Gonzalez]
> * balena-build: Add option to keep local containers [Alex Gonzalez]
> * yocto-build-env: Update Dockerfile to add host tools dependencies [Alex Gonzalez]
> * Shorten installation directory '/yocto/resin-board' to '/work' [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.11
> ### (2021-05-11)
> 
> * Substitute device type in config.js if present [Kyle Harding]
> 
> ## balena-yocto-scripts-1.12.10
> ### (2021-04-28)
> 
> * balena-build: print submodule status [Alex Gonzalez]
> * balena-build: Correctly pass development images flag and amend usage [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.9
> ### (2021-04-22)
> 
> * balena-build: Pass the API environment to the build container [Alex Gonzalez]
> * balena-lib: Add function to resolve between contract slugs and Yocto machines [Alex Gonzalez]
> * balena-build: Do not exit if no SSH_AUTH_SOCK defined [Alex Gonzalez]
> * balena-build: Fix indentation [Alex Gonzalez]
> * balena-build: Cleanup build containers and enable build output [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.8
> ### (2021-04-15)
> 
> * balena-build: Fix development image build [Alex Gonzalez]
> * jenkins_build-containers: Use a fixed length for the git short revision [Alex Gonzalez]
> * balena-lib: Do not err when sourcing without a repository [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.7
> ### (2021-04-12)
> 
> * balena-api: Improve logs when setting version [Alex Gonzalez]
> * balena-docker: Make it less verbose [Alex Gonzalez]
> * balena-deploy: Set the OS version before setting deploy directory [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.6
> ### (2021-03-30)
> 
> * include: Move include files and entry scripts into its own folder [Alex Gonzalez]
> * balena-build.sh: Move into build script [Alex Gonzalez]
> * balena-lib: Set default namespace if not defined [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.5
> ### (2021-03-30)
> 
> * balena-deploy: Shellcheck warnings [Alex Gonzalez]
> * balena-deploy-block: Adjust variables for common use [Alex Gonzalez]
> * balena-deploy-block: Fix shellcheck warnings [Alex Gonzalez]
> * balena-deploy: Adjust balena_deploy_hostapp to new balena_deploy_block entrypoint arguments [Alex Gonzalez]
> * balena-deploy.inc: Pass API environment to balena_lib_token [Alex Gonzalez]
> * balena-build: Pass an API environment to balena_lib_token [Alex Gonzalez]
> * balena-lib: Pass API environment to balena_lib_token [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.4
> ### (2021-03-29)
> 
> * balena-api: Add is_dt_private function [Alex Gonzalez]
> * balena-lib: Add several function to extract device details from device type JSON file [Alex Gonzalez]
> * balena-lib: By default only login to BaleneCloud if not token is found [Alex Gonzalez]
> * balena_deploy: Add functions to deploy Jenkins artifacts to S3 and dockerhub [Alex Gonzalez]
> * balena-deploy: Fix indentation and shellcheck warnings [Alex Gonzalez]
> * jenkins_build: Call out to script libraries functions [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.3
> ### (2021-03-26)
> 
> * balena-lib: Fix indentation to tabs [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.2
> ### (2021-03-26)
> 
> * balena-docker: Remove execution trace flag [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.1
> ### (2021-03-25)
> 
> * balena-lib: Add commonly used utility functions [Alex Gonzalez]
> * jenkins_build-containers: Allow docker login for local development [Alex Gonzalez]
> * barys: Add bitbake-args argument and make bitbake-target accept multiple arguments [Alex Gonzalez]
> * jenkins_build: Separate deploy functions [Alex Gonzalez]
> * jenkins_build: Refactor balena_lib_get_os_version [Alex Gonzalez]
> * balena-api: Add script library with API calls [Alex Gonzalez]
> * balena-push-os-version: Rename to balena-deploy-block and set the release version on deploy [Alex Gonzalez]
> * Dockerfile_balena-push-env: Refactor to use balena-deploy-block [Alex Gonzalez]
> * balena-build: Split build related functions [Alex Gonzalez]
> * jenkins_build: Separate barys build functions [Alex Gonzalez]
> * balena-deploy: Add script library for deploy logic [Alex Gonzalez]
> * jenkins_build: Use balena_deploy_hostapp from balena-deploy [Alex Gonzalez]
> 
> ## balena-yocto-scripts-1.12.0
> ### (2021-03-25)
> 
> * barys: Improve template layer matching [Kyle Harding]
> 
> ## balena-yocto-scripts-1.11.2
> ### (2021-03-22)
> 
> * jenkins_build-container: Do not overwrite environment DOCKERFILES variable if provided [Alex Gonzalez]
> * balena-lib: Rename to balena-lib.inc [Alex Gonzalez]
> * balena-lib: Rename functions with the balena_lib prefix [Alex Gonzalez]
> * jenkins_build: Use balena-lib.inc instead of balena-inc.sh [Alex Gonzalez]
> 
</details>

# v2.73.10+rev2
## (2021-04-16)

* Revert to balena-yocto-scripts v1.11.1 [Alex Gonzalez]

# v2.73.10+rev1
## (2021-04-15)

* Update meta-balena from v2.72.1 to v2.73.10 [Alex Gonzalez]
* Update  balena-yocto-scripts from v1.11.1 to v1.12.8 [Alex Gonzalez]

# v2.72.0+rev1
## (2021-03-11)

* Rename resin image types to balena [Kyle Harding]

<details>
<summary> Update meta-balena from v2.68.1 to v2.72.0 [Kyle Harding] </summary>

> ## meta-balena-2.72.0
> ### (2021-03-10)
> 
> 
> <details>
> <summary> os-config: Update os-config from v1.1.4 to v1.2.0 [Kyle Harding] </summary>
> 
>> ### os-config-1.2.0
>> #### (2021-02-23)
>> 
>> * os-config: rename flasher flag path [Kyle Harding]
>> 
> </details>
> 
> * Rename resin image types to balena [Kyle Harding]
> 
> ## meta-balena-2.71.7
> ### (2021-03-08)
> 
> * Apply aufs patches if aufs is present in kernel config [Kyle Harding]
> 
> ## meta-balena-2.71.6
> ### (2021-03-05)
> 
> * grub-efi: build required modules into grub image [Joseph Kogut]
> 
> ## meta-balena-2.71.5
> ### (2021-03-03)
> 
> * initrdscripts: always use by-uuid symlink looking for flasher rootfs [Michal Toman]
> 
> ## meta-balena-2.71.4
> ### (2021-03-01)
> 
> * Update OS test suite [Vipul Gupta (@vipulgupta2048)]
> 
> ## meta-balena-2.71.3
> ### (2021-02-26)
> 
> * balena: Make the healthcheck loading service part of balena.service [Robert Günzler]
> 
> ## meta-balena-2.71.2
> ### (2021-02-23)
> 
> * dnsmasq: enable dbus support [Kyle Harding]
> * dnsmasq: update to 2.84 with dnspooq fix [Kyle Harding]
> 
> ## meta-balena-2.71.1
> ### (2021-02-23)
> 
> * recipes-bsp: grub: install only release modules [Joseph Kogut]
> 
> ## meta-balena-2.71.0
> ### (2021-02-15)
> 
> * meta-balena-common: add grub-efi support [Joseph Kogut]
> 
> ## meta-balena-2.70.2
> ### (2021-02-12)
> 
> * Update PR template to specify test coverage in more detail [Alex Gonzalez]
> * Update codeowners [Alex Gonzalez]
> 
> ## meta-balena-2.70.1
> ### (2021-02-11)
> 
> * Add leviathan automated OS test suite [Vipul Gupta (@vipulgupta2048)]
> 
> ## meta-balena-2.70.0
> ### (2021-02-11)
> 
> * systemd/timeinit: use systemd mount unit for /etc/fake-hwclock [Mark Corbin]
> 
> ## meta-balena-2.69.1
> ### (2021-02-03)
> 
> * Update balena-supervisor from v12.3.0 to v12.3.5 [Miguel Casqueira]
> 
> ## meta-balena-2.69.0
> ### (2021-02-01)
> 
> * openvpn: remove resin-ntp-config call from upscript.sh [Mark Corbin]
> * resin-vars: trigger NTP config script on config.json changes [Mark Corbin]
> * resin-ntp-config: update script and add systemd service [Mark Corbin]
> * networkmanager: add improved dispatcher scripts for NTP handling [Mark Corbin]
> * chrony: add sourcedir support and helper script [Mark Corbin]
> 
</details>

* Update balena-yocto-scripts from v1.9.0 to v1.11.0 [Kyle Harding]

# v2.68.1+rev5
## (2021-02-19)

* Add bluetooth support [Alex Gonzalez]

# v2.68.1+rev4
## (2021-02-14)

* Add u-boot environment import/export functionality [Alex Gonzalez]
* Correct provisioning instructions for ccimx8x-sbc-pro [Alex Gonzalez]

# v2.68.1+rev3
## (2021-02-13)

* Add instructions for SD boot [Alex Gonzalez]

# v2.68.1+rev2
## (2021-02-13)

* Default to B0 / 2GB / 32bits module variants [Alex Gonzalez]

# v2.68.1+rev1
## (2021-02-13)


<details>
<summary> Update meta-balena from v2.65.1 to v2.68.1 [Alex Gonzalez] </summary>

> ## meta-balena-2.68.1
> ### (2021-01-29)
> 
> * Fix task ordering for the iwlwifi_firmware_clean task [Florin Sarbu]
> 
> ## meta-balena-2.68.0
> ### (2021-01-29)
> 
> * Update NetworkManager to 1.28.0 [Zahari Petkov]
> 
> ## meta-balena-2.67.6
> ### (2021-01-28)
> 
> * docs: mention balenaRootCA as a config.json parameter [Matthew McGinn]
> 
> ## meta-balena-2.67.5
> ### (2021-01-27)
> 
> * replace busybox ps with procps [klutchell] [Kyle Harding]
> 
> ## meta-balena-2.67.4
> ### (2021-01-27)
> 
> * Update aufs4 and aufs5 kernel patches [Florin Sarbu]
> 
> ## meta-balena-2.67.3
> ### (2021-01-15)
> 
> * kernel-headers-test: Install python dependency [Alexandru Costache]
> 
> ## meta-balena-2.67.2
> ### (2021-01-14)
> 
> * Fix pppd timeout when launched by NetworkManager [Zahari Petkov]
> 
> ## meta-balena-2.67.1
> ### (2021-01-13)
> 
> * resin-device-register: Fix post provisioning state not reported [Alexandru Costache]
> 
> ## meta-balena-2.67.0
> ### (2021-01-12)
> 
> * Update balena-supervisor from v12.2.11 to v12.3.0 [Felipe Lalanne]
> 
> ## meta-balena-2.66.3
> ### (2021-01-12)
> 
> * Respect custom CA in supervisor [Michal Toman]
> 
> ## meta-balena-2.66.2
> ### (2021-01-11)
> 
> * README: Rename resin-logo to balena-logo. [Alex Gonzalez]
> 
> ## meta-balena-2.66.1
> ### (2021-01-04)
> 
> * kernel-devsrc: use upstream recipe starting with dunfell [Kyle Harding]
> * gen_mod_headers: add missing arch headers to tools [Kyle Harding]
> 
> ## meta-balena-2.66.0
> ### (2020-12-18)
> 
> * chrony: bump to version 4.0 [Mark Corbin]
> 
</details>

# v2.65.1+rev1
## (2021-01-21)

* Add support for the ConnectCore 8X SBC Pro modules [Alex Gonzalez]
