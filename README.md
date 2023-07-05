$ dalvikvm
Class name required
~ $ dir
~ $
~ $ dalvikvm -dirdev
Unknown argument: -dirdev
dalvikvm: [options] class [argument ...]

The following standard arguments are supported:

  -classpath {string value}
  -cp {string value}
    The classpath, separated by ':'

  -D{string value} [-D{string value}...]

  -verbose:{class|collector|compiler|deopt|gc|heap|interpreter|jdwp|jit|jni|monitor|oat|profiler|signals|simulator|startup|third-party-jni|threads|verifier|verifier-debug|image|systrace-locks|plugin|agents|dex}
    Switches for advanced logging. Multiple categories can be enabled separated by ','. Eg: -verbose:class,deopt

  -help
  -h
    Print this help text.

  -showversion

  -agentpath:{/path/to/libagent.so=options} [-agentpath:{/path/to/libagent.so=options}...]
    Load native agents.
The following extended arguments are supported:

  -Xbootclasspath:{list separated by ':'}

  -Xbootclasspathfds:{integer list separated by ':'}

  -Xbootclasspathimagefds:{integer list separated by ':'}

  -Xbootclasspathvdexfds:{integer list separated by ':'}

  -Xbootclasspathoatfds:{integer list separated by ':'}

  -Xcheck:jni

  -Xms{Memory with granularity of 1024 bytes}

  -Xmx{Memory with granularity of 1024 bytes}

  -Xss{Memory with granularity of 1 bytes}

  -Xint
The following Dalvik arguments are supported:

  -Xzygote
    Start as zygote

  -Xjnitrace:{string value}

  -Xgc:{MS|nonconccurent|concurrent|CMS|SS|CC|[no]preverify[_rosalloc]|[no]presweepingverify[_rosalloc]|[no]generation_cc|[no]postverify[_rosalloc]|[no]gcstress|measure|[no]precisce|[no]verifycardtable}

  -XX:HeapGrowthLimit={Memory with granularity of 1024 bytes}

  -XX:HeapMinFree={Memory with granularity of 1024 bytes}

  -XX:HeapMaxFree={Memory with granularity of 1024 bytes}

  -XX:NonMovingSpaceCapacity={Memory with granularity of 1024 bytes}

  -XX:HeapTargetUtilization={double value}

  -XX:ForegroundHeapGrowthMultiplier={double value}

  -XX:LowMemoryMode

  -Xprofile:{threadcpuclock|wallclock|dualclock}

  -Xjitthreshold:{unsigned integer value}
The following ART arguments are supported:

  -Ximage:{list separated by ':'}

  -Xforcejitzygote

  -Xprimaryzygote

  -Xbootclasspath-locations:{list separated by ':'}

  -Xjniopts:forcecopy

  -XjdwpProvider:{none|adbconnection|default}

  -XjdwpOptions:OPTION[,OPTION...]
    JDWP options. Eg suspend=n,server=y.

  -XX:StopForNativeAllocs={Memory with granularity of 1024 bytes}

  -XX:ParallelGCThreads={unsigned integer value}

  -XX:ConcGCThreads={unsigned integer value}

  -XX:FinalizerTimeoutMs={unsigned integer value}

  -XX:MaxSpinsBeforeThinLockInflation={unsigned integer value}

  -XX:LongPauseLogThreshold={millisecond value}

  -XX:LongGCLogThreshold={millisecond value}

  -XX:DumpGCPerformanceOnShutdown

  -XX:DumpRegionInfoBeforeGC

  -XX:DumpRegionInfoAfterGC

  -XX:DumpJITInfoOnShutdown

  -XX:IgnoreMaxFootprint

  -XX:AlwaysLogExplicitGcs:{false|true}
    Allows one to control the logging of explicit GCs. Defaults to 'true'

  -XX:UseTLAB

  -XX:EnableHSpaceCompactForOOM
  -XX:DisableHSpaceCompactForOOM

  -XX:DumpNativeStackOnSigQuit:{false|true}

  -XX:MadviseRandomAccess:{false|true}

  -XMadviseWillNeedVdexFileSize:{unsigned integer value}

  -XMadviseWillNeedOdexFileSize:{unsigned integer value}

  -XMadviseWillNeedArtFileSize:{unsigned integer value}

  -Xusejit:{false|true}

  -Xuseprofiledjit:{false|true}

  -Xjitinitialsize:{Memory with granularity of 1024 bytes}

  -Xjitmaxsize:{Memory with granularity of 1024 bytes}

  -Xjitwarmupthreshold:{unsigned integer value}

  -Xjitprithreadweight:{unsigned integer value}

  -Xjittransitionweight:{unsigned integer value}

  -Xjitpthreadpriority:{integer value}

  -Xjitzygotepthreadpriority:{integer value}

  -Xjitsaveprofilinginfo [-Xjitsaveprofilinginfo...]

  -Xps-{string|unsigned integer} [-Xps-{string|unsigned integer}...]
  -Xps-min-save-period-ms:{string|unsigned integer} [-Xps-min-save-period-ms:{string|unsigned integer}...]
  -Xps-min-first-save-ms:{string|unsigned integer} [-Xps-min-first-save-ms:{string|unsigned integer}...]
  -Xps-save-resolved-classes-delayed-ms:{string|unsigned integer} [-Xps-save-resolved-classes-delayed-ms:{string|unsigned integer}...]
  -Xps-hot-startup-method-samples:{string|unsigned integer} [-Xps-hot-startup-method-samples:{string|unsigned integer}...]
  -Xps-min-methods-to-save:{string|unsigned integer} [-Xps-min-methods-to-save:{string|unsigned integer}...]
  -Xps-min-classes-to-save:{string|unsigned integer} [-Xps-min-classes-to-save:{string|unsigned integer}...]
  -Xps-min-notification-before-wake:{string|unsigned integer} [-Xps-min-notification-before-wake:{string|unsigned integer}...]
  -Xps-max-notification-before-wake:{string|unsigned integer} [-Xps-max-notification-before-wake:{string|unsigned integer}...]
  -Xps-profile-path:{string|unsigned integer} [-Xps-profile-path:{string|unsigned integer}...]
    profile-saver options -Xps-<key>:<value>

  -XX:HspaceCompactForOOMMinIntervalMs={millisecond value}

  -Xrelocate
  -Xnorelocate

  -Ximage-dex2oat
  -Xnoimage-dex2oat

  -XX:LargeObjectSpace={disabled|freelist|map}

  -XX:LargeObjectThreshold={Memory with granularity of 1 bytes}

  -XX:BackgroundGC={HSpaceCompact|MS|nonconccurent|CMS|concurrent|SS|CC}

  -XX:+DisableExplicitGC

  -Xlockprofthreshold:{unsigned integer value}

  -Xstackdumplockprofthreshold:{unsigned integer value}

  -Xmethod-trace

  -Xmethod-trace-file:{string value}

  -Xmethod-trace-file-size:{unsigned integer value}

  -Xmethod-trace-stream

  -Xcompiler:{string value}

  -Xcompiler-option {string value} [-Xcompiler-option {string value}...]

  -Ximage-compiler-option {string value} [-Ximage-compiler-option {string value}...]

  -Xverify:{none|remote|all|softfail}

  -XX:NativeBridge={string value}

  -Xzygote-max-boot-retry={unsigned integer value}

  -Xno-sig-chain

  --cpu-abilist={string value}

  -Xfingerprint:{string value}

  -Xexperimental:{none} [-Xexperimental:{none}...]

  -Xforce-nb-testing

  -Xplugin:{/path/to/libplugin.so} [-Xplugin:{/path/to/libplugin.so}...]
    Load and initialize the specified art-plugin.

  -XX:ThreadSuspendTimeout={millisecond value}

  -XX:MonitorTimeoutEnable={false|true}

  -XX:MonitorTimeout={integer value}

  -XX:GlobalRefAllocStackTraceLimit={unsigned integer value}

  -XX:SlowDebug={false|true}

  -Xtarget-sdk-version:{unsigned integer value}

  -Xhidden-api-policy:{disabled|just-warn|enabled}

  -Xcore-platform-api-policy:{disabled|just-warn|enabled}

  -Xuse-stderr-logger

  -Xonly-use-system-oat-files

  -Xdeny-art-apex-data-files

  -Xverifier-logging-threshold={unsigned integer value}

  -XX:FastClassNotFoundException={false|true}

  -Xopaque-jni-ids:{true|false|swapable|pointer|indices|default}
    Control the representation of jmethodID and jfieldID values

  -Xauto-promote-opaque-jni-ids:{true|false}

  -XX:VerifierMissingKThrowFatal={false|true}

  -XX:ForceJavaZygoteForkLoop={false|true}

  -XX:PerfettoHprof={false|true}

  -XX:PerfettoJavaHeapStackProf={false|true}

  -Xmetrics-format:{string value}

  -Xmetrics-write-to-file:{string value}

  -Xmetrics-write-to-logcat:{true|false|1|0|y|n|yes|no|on|off}

  -Xmetrics-write-to-statsd:{true|false|1|0|y|n|yes|no|on|off}

  -Xmetrics-reporting-num-mods-server:{unsigned integer value}

  -Xmetrics-reporting-num-mods:{unsigned integer value}

  -Xmetrics-reporting-mods-server:{unsigned integer value}

  -Xmetrics-reporting-mods:{unsigned integer value}

  -Xmetrics-reporting-spec-server:{string value}

  -Xmetrics-reporting-spec:{string value}

  -Xmy-feature-test-flag:{integer value}
The following arguments are ignored for compatibility:
  -ea
  -da
  -enableassertions
  -disableassertions
  --runtime-arg
  -esa
  -dsa
  -enablesystemassertions
  -disablesystemassertions
  -Xrs
  -Xint:_
  -Xdexopt:_
  -Xnoquithandler
  -Xjnigreflimit:_
  -Xgenregmap
  -Xnogenregmap
  -Xverifyopt:_
  -Xcheckdexsum
  -Xincludeselectedop
  -Xjitop:_
  -Xincludeselectedmethod
  -Xjitblocking
  -Xjitmethod:_
  -Xjitclass:_
  -Xjitoffset:_
  -Xjitosrthreshold:_
  -Xjitconfig:_
  -Xjitcheckcg
  -Xjitverbose
  -Xjitprofile
  -Xjitdisableopt
  -Xjitsuspendpoll
  -XX:mainThreadStackSize=_
  
