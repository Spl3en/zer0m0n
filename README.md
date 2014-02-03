zer0m0n v0.2 (DEVELOPMENT BRANCH)
=================================

Changes :
+ ZwDeviceIoControlFile hook
+ ZwCreateMutant hook
+ ZwDelayExecution hook
+ ZwTerminateProcess hook
+ Fixed deadlock issue (FltSendMessage infinite wait switched to 100ms timeout)
+ Fixed performance issues (drop) using userland app multithreading

Todo :
+ Use inverted IRP calls with kernel buffer instead of filter comm. ports :]
+ Handle SSDT hooks race conditions (perform legitimate calls with copied parameters)
+ Handle ZwTerminateProcess race condition (notify analyzer.py of process termination)
+ Add anti-detection features (cuckoo / VM files/process/reg/connections)
+ Hide thread listing
+ Get ZwCreateProcess* filename parameter
+ Handle machine poweroff
+ Handle driver execution
+ Add monitored functions / events
+ Handle file deletion
+ Eliminate bugs :]
+ Log registry callbacks return values
+ Add signatures
+ win7 x86 support
+ x64 support (get rid of SSDT hooks)
+ etc.
