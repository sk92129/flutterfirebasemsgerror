-------------------------------------
Translated Report (Full Report Below)
-------------------------------------

Incident Identifier: 70EF603D-03AD-4ECC-9532-0A3BEBD2ADE8
CrashReporter Key:   D6CD3DE7-33F5-50C1-9186-F4A958BE619A
Hardware Model:      Mac14,9
Process:             Runner [97214]
Path:                /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Runner
Identifier:          com.kangengineering.universalapp.uniapp
Version:             1.0.0 (1)
Code Type:           ARM-64 (Native)
Role:                Foreground
Parent Process:      launchd_sim [39128]
Coalition:           com.apple.CoreSimulator.SimDevice.2252DDC0-C915-4B0C-8C71-B97C2BC60A03 [65786]
Responsible Process: SimulatorTrampoline [2442]

Date/Time:           2025-07-11 23:00:05.3229 -0700
Launch Time:         2025-07-11 23:00:04.6289 -0700
OS Version:          macOS 15.5 (24F74)
Release Type:        User
Report Version:      104

Exception Type:  EXC_CRASH (SIGABRT)
Exception Codes: 0x0000000000000000, 0x0000000000000000
Termination Reason: SIGNAL 6 Abort trap: 6
Terminating Process: Runner [97214]

Triggered by Thread:  0

Last Exception Backtrace:
0   CoreFoundation                	       0x1804eb1d0 __exceptionPreprocess + 160
1   libobjc.A.dylib               	       0x18009bf84 objc_exception_throw + 72
2   CoreFoundation                	       0x1804eb0ec -[NSException initWithCoder:] + 0
3   FirebaseCore                  	       0x104ff932c +[FIRApp configure] + 120 (FIRApp.m:115)
4   Runner.debug.dylib            	       0x104eb5d14 AppDelegate.application(_:didFinishLaunchingWithOptions:) + 72 (AppDelegate.swift:13)
5   Runner.debug.dylib            	       0x104eb6050 @objc AppDelegate.application(_:didFinishLaunchingWithOptions:) + 220
6   UIKitCore                     	       0x186220abc -[UIApplication _handleDelegateCallbacksWithOptions:isSuspended:restoreState:] + 332
7   UIKitCore                     	       0x186221ff8 -[UIApplication _callInitializationDelegatesWithActions:forScene:payload:fromOriginatingProcess:] + 3036
8   UIKitCore                     	       0x186227438 -[UIApplication _runWithMainScene:transitionContext:completion:] + 800
9   UIKitCore                     	       0x1857de898 -[_UISceneLifecycleMultiplexer completeApplicationLaunchWithFBSScene:transitionContext:] + 88
10  UIKitCore                     	       0x185d9a150 _UIScenePerformActionsWithLifecycleActionMask + 96
11  UIKitCore                     	       0x1857df174 __101-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]_block_invoke + 224
12  UIKitCore                     	       0x1857decd0 -[_UISceneLifecycleMultiplexer _performBlock:withApplicationOfDeactivationReasons:fromReasons:] + 204
13  UIKitCore                     	       0x1857defa8 -[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:] + 576
14  UIKitCore                     	       0x1857de9c0 -[_UISceneLifecycleMultiplexer uiScene:transitionedFromState:withTransitionContext:] + 240
15  UIKitCore                     	       0x1857ea8c4 __186-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]_block_invoke + 140
16  UIKitCore                     	       0x185c85e1c +[BSAnimationSettings(UIKit) tryAnimatingWithSettings:fromCurrentState:actions:completion:] + 656
17  UIKitCore                     	       0x185db285c _UISceneSettingsDiffActionPerformChangesWithTransitionContextAndCompletion + 196
18  UIKitCore                     	       0x1857ea5d0 -[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:] + 288
19  UIKitCore                     	       0x185611054 __64-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]_block_invoke.190 + 612
20  UIKitCore                     	       0x18560fdf4 -[UIScene _emitSceneSettingsUpdateResponseForCompletion:afterSceneUpdateWork:] + 200
21  UIKitCore                     	       0x185610cd4 -[UIScene scene:didUpdateWithDiff:transitionContext:completion:] + 220
22  UIKitCore                     	       0x1862261a4 -[UIApplication workspace:didCreateScene:withTransitionContext:completion:] + 452
23  UIKitCore                     	       0x185cb13ec -[UIApplicationSceneClientAgent scene:didInitializeWithEvent:completion:] + 260
24  FrontBoardServices            	       0x188494188 __95-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]_block_invoke + 304
25  FrontBoardServices            	       0x1884945f4 -[FBSScene _callOutQueue_maybeCoalesceClientSettingsUpdates:] + 116
26  FrontBoardServices            	       0x188493fdc -[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:] + 408
27  FrontBoardServices            	       0x1884ff6e4 __93-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]_block_invoke.274 + 232
28  FrontBoardServices            	       0x1884a162c -[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:] + 160
29  FrontBoardServices            	       0x1884bf76c -[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:] + 392
30  FrontBoardServices            	       0x1884c0e40 __92-[FBSWorkspaceScenesClient createSceneWithIdentity:parameters:transitionContext:completion:]_block_invoke_2 + 204
31  FrontBoardServices            	       0x1884a162c -[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:] + 160
32  libdispatch.dylib             	       0x1801d34b0 _dispatch_client_callout + 12
33  libdispatch.dylib             	       0x1801bdb0c _dispatch_block_invoke_direct + 376
34  BoardServices                 	       0x187f0d73c __BSSERVICEMAINRUNLOOPQUEUE_IS_CALLING_OUT_TO_A_BLOCK__ + 44
35  BoardServices                 	       0x187f0c76c BSServiceMainRunLoopSourceHandler + 180
36  CoreFoundation                	       0x180445b20 __CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__ + 24
37  CoreFoundation                	       0x180445a68 __CFRunLoopDoSource0 + 168
38  CoreFoundation                	       0x180445250 __CFRunLoopDoSources0 + 312
39  CoreFoundation                	       0x1804443a8 __CFRunLoopRun + 756
40  CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
41  GraphicsServices              	       0x1928d19bc GSEventRunModal + 116
42  UIKitCore                     	       0x186224480 -[UIApplication _run] + 772
43  UIKitCore                     	       0x186228650 UIApplicationMain + 124
44  UIKitCore                     	       0x1854c7d58 0x185158000 + 3603800
45  Runner.debug.dylib            	       0x104eb621c static UIApplicationDelegate.main() + 128
46  Runner.debug.dylib            	       0x104eb618c static AppDelegate.$main() + 44
47  Runner.debug.dylib            	       0x104eb6298 __debug_main_executable_dylib_entry_point + 28
48  ???                           	       0x104f093d0 ???
49  dyld                          	       0x1051f2b98 start + 6076

Thread 0 Crashed::  Dispatch queue: com.apple.main-thread
0   libsystem_kernel.dylib        	       0x1054fc874 __pthread_kill + 8
1   libsystem_pthread.dylib       	       0x10542e2ec pthread_kill + 264
2   libsystem_c.dylib             	       0x1801ad9b8 abort + 100
3   libc++abi.dylib               	       0x1802f326c __abort_message + 128
4   libc++abi.dylib               	       0x1802e31a4 demangling_terminate_handler() + 268
5   libobjc.A.dylib               	       0x180077218 _objc_terminate() + 124
6   libc++abi.dylib               	       0x1802f2758 std::__terminate(void (*)()) + 12
7   libc++abi.dylib               	       0x1802f57c0 __cxxabiv1::failed_throw(__cxxabiv1::__cxa_exception*) + 32
8   libc++abi.dylib               	       0x1802f57a0 __cxa_throw + 88
9   libobjc.A.dylib               	       0x18009c0bc objc_exception_throw + 384
10  CoreFoundation                	       0x1804eb0ec +[NSException raise:format:] + 124
11  FirebaseCore                  	       0x104ff932c +[FIRApp configure] + 120 (FIRApp.m:110)
12  Runner.debug.dylib            	       0x104eb5d14 AppDelegate.application(_:didFinishLaunchingWithOptions:) + 72 (AppDelegate.swift:12)
13  Runner.debug.dylib            	       0x104eb6050 @objc AppDelegate.application(_:didFinishLaunchingWithOptions:) + 220
14  UIKitCore                     	       0x186220abc -[UIApplication _handleDelegateCallbacksWithOptions:isSuspended:restoreState:] + 332
15  UIKitCore                     	       0x186221ff8 -[UIApplication _callInitializationDelegatesWithActions:forScene:payload:fromOriginatingProcess:] + 3036
16  UIKitCore                     	       0x186227438 -[UIApplication _runWithMainScene:transitionContext:completion:] + 800
17  UIKitCore                     	       0x1857de898 -[_UISceneLifecycleMultiplexer completeApplicationLaunchWithFBSScene:transitionContext:] + 88
18  UIKitCore                     	       0x185d9a150 _UIScenePerformActionsWithLifecycleActionMask + 96
19  UIKitCore                     	       0x1857df174 __101-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]_block_invoke + 224
20  UIKitCore                     	       0x1857decd0 -[_UISceneLifecycleMultiplexer _performBlock:withApplicationOfDeactivationReasons:fromReasons:] + 204
21  UIKitCore                     	       0x1857defa8 -[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:] + 576
22  UIKitCore                     	       0x1857de9c0 -[_UISceneLifecycleMultiplexer uiScene:transitionedFromState:withTransitionContext:] + 240
23  UIKitCore                     	       0x1857ea8c4 __186-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]_block_invoke + 140
24  UIKitCore                     	       0x185c85e1c +[BSAnimationSettings(UIKit) tryAnimatingWithSettings:fromCurrentState:actions:completion:] + 656
25  UIKitCore                     	       0x185db285c _UISceneSettingsDiffActionPerformChangesWithTransitionContextAndCompletion + 196
26  UIKitCore                     	       0x1857ea5d0 -[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:] + 288
27  UIKitCore                     	       0x185611054 __64-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]_block_invoke.190 + 612
28  UIKitCore                     	       0x18560fdf4 -[UIScene _emitSceneSettingsUpdateResponseForCompletion:afterSceneUpdateWork:] + 200
29  UIKitCore                     	       0x185610cd4 -[UIScene scene:didUpdateWithDiff:transitionContext:completion:] + 220
30  UIKitCore                     	       0x1862261a4 -[UIApplication workspace:didCreateScene:withTransitionContext:completion:] + 452
31  UIKitCore                     	       0x185cb13ec -[UIApplicationSceneClientAgent scene:didInitializeWithEvent:completion:] + 260
32  FrontBoardServices            	       0x188494188 __95-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]_block_invoke + 304
33  FrontBoardServices            	       0x1884945f4 -[FBSScene _callOutQueue_maybeCoalesceClientSettingsUpdates:] + 116
34  FrontBoardServices            	       0x188493fdc -[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:] + 408
35  FrontBoardServices            	       0x1884ff6e4 __93-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]_block_invoke.274 + 232
36  FrontBoardServices            	       0x1884a162c -[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:] + 160
37  FrontBoardServices            	       0x1884bf76c -[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:] + 392
38  FrontBoardServices            	       0x1884c0e40 __92-[FBSWorkspaceScenesClient createSceneWithIdentity:parameters:transitionContext:completion:]_block_invoke_2 + 204
39  FrontBoardServices            	       0x1884a162c -[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:] + 160
40  libdispatch.dylib             	       0x1801d34b0 _dispatch_client_callout + 12
41  libdispatch.dylib             	       0x1801bdb0c _dispatch_block_invoke_direct + 376
42  BoardServices                 	       0x187f0d73c __BSSERVICEMAINRUNLOOPQUEUE_IS_CALLING_OUT_TO_A_BLOCK__ + 44
43  BoardServices                 	       0x187f0c76c BSServiceMainRunLoopSourceHandler + 180
44  CoreFoundation                	       0x180445b20 __CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__ + 24
45  CoreFoundation                	       0x180445a68 __CFRunLoopDoSource0 + 168
46  CoreFoundation                	       0x180445250 __CFRunLoopDoSources0 + 312
47  CoreFoundation                	       0x1804443a8 __CFRunLoopRun + 756
48  CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
49  GraphicsServices              	       0x1928d19bc GSEventRunModal + 116
50  UIKitCore                     	       0x186224480 -[UIApplication _run] + 772
51  UIKitCore                     	       0x186228650 UIApplicationMain + 124
52  UIKitCore                     	       0x1854c7d58 0x185158000 + 3603800
53  Runner.debug.dylib            	       0x104eb621c static UIApplicationDelegate.main() + 128
54  Runner.debug.dylib            	       0x104eb618c static AppDelegate.$main() + 44
55  Runner.debug.dylib            	       0x104eb6298 __debug_main_executable_dylib_entry_point + 28
56  ???                           	       0x104f093d0 ???
57  dyld                          	       0x1051f2b98 start + 6076

Thread 1:
0   libsystem_pthread.dylib       	       0x105429984 start_wqthread + 0

Thread 2::  Dispatch queue: com.apple.libtrace.state.block-list
0   libsystem_kernel.dylib        	       0x1054f6770 __ulock_wait + 8
1   libdispatch.dylib             	       0x1801ba5b0 _dlock_wait + 52
2   libdispatch.dylib             	       0x1801ba3bc _dispatch_thread_event_wait_slow + 52
3   libdispatch.dylib             	       0x1801c9368 __DISPATCH_WAIT_FOR_QUEUE__ + 392
4   libdispatch.dylib             	       0x1801c8e64 _dispatch_sync_f_slow + 160
5   libsystem_trace.dylib         	       0x1800f2f90 ___os_state_request_for_self_block_invoke + 340
6   libdispatch.dylib             	       0x1801b87a8 _dispatch_call_block_and_release + 24
7   libdispatch.dylib             	       0x1801d34b0 _dispatch_client_callout + 12
8   libdispatch.dylib             	       0x1801c1c28 _dispatch_lane_serial_drain + 984
9   libdispatch.dylib             	       0x1801c26e8 _dispatch_lane_invoke + 396
10  libdispatch.dylib             	       0x1801cd534 _dispatch_root_queue_drain_deferred_wlh + 288
11  libdispatch.dylib             	       0x1801ccc74 _dispatch_workloop_worker_thread + 692
12  libsystem_pthread.dylib       	       0x10542abcc _pthread_wqthread + 288
13  libsystem_pthread.dylib       	       0x10542998c start_wqthread + 8

Thread 3::  Dispatch queue: com.apple.UIKit.KeyboardManagement
0   libsystem_kernel.dylib        	       0x1054f6770 __ulock_wait + 8
1   libdispatch.dylib             	       0x1801ba5b0 _dlock_wait + 52
2   libdispatch.dylib             	       0x1801ba3bc _dispatch_thread_event_wait_slow + 52
3   libdispatch.dylib             	       0x1801c9368 __DISPATCH_WAIT_FOR_QUEUE__ + 392
4   libdispatch.dylib             	       0x1801c8e64 _dispatch_sync_f_slow + 160
5   UIKitCore                     	       0x186063994 __37-[_UIRemoteKeyboards startConnection]_block_invoke.388 + 116
6   CoreFoundation                	       0x1804f1ba0 __invoking___ + 144
7   CoreFoundation                	       0x1804eed50 -[NSInvocation invoke] + 276
8   Foundation                    	       0x1811d7c60 <deduplicated_symbol> + 12
9   Foundation                    	       0x1811d78cc -[NSXPCConnection _decodeAndInvokeReplyBlockWithEvent:sequence:replyInfo:] + 484
10  Foundation                    	       0x1811db7b4 __88-[NSXPCConnection _sendInvocation:orArguments:count:methodSignature:selector:withProxy:]_block_invoke_5 + 184
11  libxpc.dylib                  	       0x180114924 _xpc_connection_reply_callout + 60
12  libxpc.dylib                  	       0x1801078bc _xpc_connection_call_reply_async + 92
13  libdispatch.dylib             	       0x1801d34d8 <deduplicated_symbol> + 12
14  libdispatch.dylib             	       0x1801d7c04 _dispatch_mach_msg_async_reply_invoke + 508
15  libdispatch.dylib             	       0x1801c1980 _dispatch_lane_serial_drain + 304
16  libdispatch.dylib             	       0x1801c26e8 _dispatch_lane_invoke + 396
17  libdispatch.dylib             	       0x1801cd534 _dispatch_root_queue_drain_deferred_wlh + 288
18  libdispatch.dylib             	       0x1801ccc74 _dispatch_workloop_worker_thread + 692
19  libsystem_pthread.dylib       	       0x10542abcc _pthread_wqthread + 288
20  libsystem_pthread.dylib       	       0x10542998c start_wqthread + 8

Thread 4:
0   libsystem_pthread.dylib       	       0x105429984 start_wqthread + 0

Thread 5:: com.apple.uikit.eventfetch-thread
0   libsystem_kernel.dylib        	       0x1054f4b70 mach_msg2_trap + 8
1   libsystem_kernel.dylib        	       0x105505fac mach_msg2_internal + 72
2   libsystem_kernel.dylib        	       0x1054fcc28 mach_msg_overwrite + 480
3   libsystem_kernel.dylib        	       0x1054f4ed8 mach_msg + 20
4   CoreFoundation                	       0x180445380 __CFRunLoopServiceMachPort + 156
5   CoreFoundation                	       0x180444514 __CFRunLoopRun + 1120
6   CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
7   Foundation                    	       0x1810f37e0 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 208
8   Foundation                    	       0x1810f3a00 -[NSRunLoop(NSRunLoop) runUntilDate:] + 60
9   UIKitCore                     	       0x1862db004 -[UIEventFetcher threadMain] + 408
10  Foundation                    	       0x18111a6d4 __NSThread__start__ + 716
11  libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
12  libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 6:: io.flutter.1.raster
0   libsystem_kernel.dylib        	       0x1054f4b70 mach_msg2_trap + 8
1   libsystem_kernel.dylib        	       0x105505fac mach_msg2_internal + 72
2   libsystem_kernel.dylib        	       0x1054fcc28 mach_msg_overwrite + 480
3   libsystem_kernel.dylib        	       0x1054f4ed8 mach_msg + 20
4   CoreFoundation                	       0x180445380 __CFRunLoopServiceMachPort + 156
5   CoreFoundation                	       0x180444514 __CFRunLoopRun + 1120
6   CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
7   Flutter                       	       0x108272438 fml::MessageLoopDarwin::Run() + 88
8   Flutter                       	       0x10826b804 fml::MessageLoopImpl::DoRun() + 40
9   Flutter                       	       0x1082710d0 std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()() + 184
10  Flutter                       	       0x108270da4 fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*) + 36
11  libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
12  libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 7:: io.flutter.1.io
0   libsystem_kernel.dylib        	       0x1054f4b70 mach_msg2_trap + 8
1   libsystem_kernel.dylib        	       0x105505fac mach_msg2_internal + 72
2   libsystem_kernel.dylib        	       0x1054fcc28 mach_msg_overwrite + 480
3   libsystem_kernel.dylib        	       0x1054f4ed8 mach_msg + 20
4   CoreFoundation                	       0x180445380 __CFRunLoopServiceMachPort + 156
5   CoreFoundation                	       0x180444514 __CFRunLoopRun + 1120
6   CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
7   Flutter                       	       0x108272438 fml::MessageLoopDarwin::Run() + 88
8   Flutter                       	       0x10826b804 fml::MessageLoopImpl::DoRun() + 40
9   Flutter                       	       0x1082710d0 std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()() + 184
10  Flutter                       	       0x108270da4 fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*) + 36
11  libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
12  libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 8:: io.flutter.1.profiler
0   libsystem_kernel.dylib        	       0x1054f4b70 mach_msg2_trap + 8
1   libsystem_kernel.dylib        	       0x105505fac mach_msg2_internal + 72
2   libsystem_kernel.dylib        	       0x1054fcc28 mach_msg_overwrite + 480
3   libsystem_kernel.dylib        	       0x1054f4ed8 mach_msg + 20
4   CoreFoundation                	       0x180445380 __CFRunLoopServiceMachPort + 156
5   CoreFoundation                	       0x180444514 __CFRunLoopRun + 1120
6   CoreFoundation                	       0x18043f458 _CFRunLoopRunSpecificWithOptions + 496
7   Flutter                       	       0x108272438 fml::MessageLoopDarwin::Run() + 88
8   Flutter                       	       0x10826b804 fml::MessageLoopImpl::DoRun() + 40
9   Flutter                       	       0x1082710d0 std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()() + 184
10  Flutter                       	       0x108270da4 fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*) + 36
11  libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
12  libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 9:: io.worker.1
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eab8 _pthread_cond_wait + 976
2   Flutter                       	       0x108248958 std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&) + 24
3   Flutter                       	       0x108267e34 fml::ConcurrentMessageLoop::WorkerMain() + 140
4   Flutter                       	       0x108268760 void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*) + 212
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 10:: io.worker.2
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eab8 _pthread_cond_wait + 976
2   Flutter                       	       0x108248958 std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&) + 24
3   Flutter                       	       0x108267e34 fml::ConcurrentMessageLoop::WorkerMain() + 140
4   Flutter                       	       0x108268760 void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*) + 212
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 11:: io.worker.3
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eab8 _pthread_cond_wait + 976
2   Flutter                       	       0x108248958 std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&) + 24
3   Flutter                       	       0x108267e34 fml::ConcurrentMessageLoop::WorkerMain() + 140
4   Flutter                       	       0x108268760 void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*) + 212
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 12:: io.worker.4
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eab8 _pthread_cond_wait + 976
2   Flutter                       	       0x108248958 std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&) + 24
3   Flutter                       	       0x108267e34 fml::ConcurrentMessageLoop::WorkerMain() + 140
4   Flutter                       	       0x108268760 void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*) + 212
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 13:: dart:io EventHandler
0   libsystem_kernel.dylib        	       0x1054fa670 kevent + 8
1   Flutter                       	       0x1086b5df8 dart::bin::EventHandlerImplementation::EventHandlerEntry(unsigned long) + 300
2   Flutter                       	       0x1086d1f50 dart::bin::ThreadStart(void*) + 88
3   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
4   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 14:: Dart Profiler ThreadInterrupter
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eab8 _pthread_cond_wait + 976
2   Flutter                       	       0x10871d658 dart::ConditionVariable::WaitMicros(dart::Mutex*, long long) + 128
3   Flutter                       	       0x10887a5f4 dart::ThreadInterrupter::ThreadMain(unsigned long) + 328
4   Flutter                       	       0x108832024 dart::ThreadStart(void*) + 204
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 15:: Dart Profiler SampleBlockProcessor
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eae4 _pthread_cond_wait + 1020
2   Flutter                       	       0x10871d648 dart::ConditionVariable::WaitMicros(dart::Mutex*, long long) + 112
3   Flutter                       	       0x108836af0 dart::SampleBlockProcessor::ThreadMain(unsigned long) + 168
4   Flutter                       	       0x108832024 dart::ThreadStart(void*) + 204
5   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
6   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 16:: DartWorker
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eae4 _pthread_cond_wait + 1020
2   Flutter                       	       0x10871d648 dart::ConditionVariable::WaitMicros(dart::Mutex*, long long) + 112
3   Flutter                       	       0x10887b36c dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*) + 508
4   Flutter                       	       0x10887b4c4 dart::ThreadPool::Worker::Main(unsigned long) + 116
5   Flutter                       	       0x108832024 dart::ThreadStart(void*) + 204
6   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
7   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 17:
0   libsystem_pthread.dylib       	       0x105429984 start_wqthread + 0

Thread 18:: DartWorker
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eae4 _pthread_cond_wait + 1020
2   Flutter                       	       0x10871d648 dart::ConditionVariable::WaitMicros(dart::Mutex*, long long) + 112
3   Flutter                       	       0x10887b36c dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*) + 508
4   Flutter                       	       0x10887b4c4 dart::ThreadPool::Worker::Main(unsigned long) + 116
5   Flutter                       	       0x108832024 dart::ThreadStart(void*) + 204
6   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
7   libsystem_pthread.dylib       	       0x105429998 thread_start + 8

Thread 19:: DartWorker
0   libsystem_kernel.dylib        	       0x1054f8014 __psynch_cvwait + 8
1   libsystem_pthread.dylib       	       0x10542eae4 _pthread_cond_wait + 1020
2   Flutter                       	       0x10871d648 dart::ConditionVariable::WaitMicros(dart::Mutex*, long long) + 112
3   Flutter                       	       0x10877b88c dart::MutatorThreadPool::OnEnterIdleLocked(dart::MutexLocker*, dart::ThreadPool::Worker*) + 152
4   Flutter                       	       0x10887b1ec dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*) + 124
5   Flutter                       	       0x10887b4c4 dart::ThreadPool::Worker::Main(unsigned long) + 116
6   Flutter                       	       0x108832024 dart::ThreadStart(void*) + 204
7   libsystem_pthread.dylib       	       0x10542e5f0 _pthread_start + 104
8   libsystem_pthread.dylib       	       0x105429998 thread_start + 8


Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x0000000000000000   x1: 0x0000000000000000   x2: 0x0000000000000000   x3: 0x0000000000000000
    x4: 0x00000001802f6cab   x5: 0x000000016afa2470   x6: 0x000000000000006e   x7: 0x0000000000000000
    x8: 0x0000000105294200   x9: 0x354a4ff519d84e2c  x10: 0x0000000000000051  x11: 0x000000000000000b
   x12: 0x000000000000000b  x13: 0x000000018070baf4  x14: 0x00000000000007fb  x15: 0x000000009ac3480c
   x16: 0x0000000000000148  x17: 0x000000009ae34011  x18: 0x0000000000000000  x19: 0x0000000000000006
   x20: 0x0000000000000103  x21: 0x00000001052942e0  x22: 0x00000001f2cf3000  x23: 0x0000000000000000
   x24: 0x0000000000000000  x25: 0x00000001f2f0b000  x26: 0x00000001f2ec6000  x27: 0x000000002b870064
   x28: 0x0000000000000010   fp: 0x000000016afa23e0   lr: 0x000000010542e2ec
    sp: 0x000000016afa23c0   pc: 0x00000001054fc874 cpsr: 0x40001000
   far: 0x0000000000000000  esr: 0x56000080  Address size fault

Binary Images:
       0x1051ec000 -        0x105287fff dyld (*) <9cf0401a-a938-389e-a77d-9e9608076ccf> /usr/lib/dyld
       0x104e58000 -        0x104e5bfff com.kangengineering.universalapp.uniapp (1.0.0) <4dbd5000-44a4-3f9b-930e-58f944fc5bdb> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Runner
       0x104eb4000 -        0x104ed3fff Runner.debug.dylib (*) <e8a0ad9f-a387-3e8a-ac25-aaac11c07124> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Runner.debug.dylib
       0x104fc4000 -        0x104fd7fff org.cocoapods.FBLPromises (2.4.0) <816d9f36-de82-38b4-b148-f613efc7a3d4> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/FBLPromises.framework/FBLPromises
       0x104ff8000 -        0x10500bfff org.cocoapods.FirebaseCore (11.15.0) <e7e3724f-2488-3765-bf88-6200ae787e5c> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/FirebaseCore.framework/FirebaseCore
       0x1050a8000 -        0x1050cffff org.cocoapods.FirebaseCoreInternal (11.15.0) <a4f2fa2f-c540-393b-a11c-c3b53dc27f62> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/FirebaseCoreInternal.framework/FirebaseCoreInternal
       0x104e70000 -        0x104e8bfff org.cocoapods.FirebaseInstallations (11.15.0) <05c04aa7-e5bc-32f3-8ea8-d32f7b76ed3e> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/FirebaseInstallations.framework/FirebaseInstallations
       0x10531c000 -        0x105363fff org.cocoapods.FirebaseMessaging (11.15.0) <086af4b4-718c-3710-aacc-600a5c29e2f7> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/FirebaseMessaging.framework/FirebaseMessaging
       0x105120000 -        0x105153fff org.cocoapods.GoogleDataTransport (10.1.0) <cdb43475-0dc1-3609-981a-ee87e1b1c04b> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/GoogleDataTransport.framework/GoogleDataTransport
       0x10518c000 -        0x1051affff org.cocoapods.GoogleUtilities (8.1.0) <2075202e-6e64-3d62-a63b-0a5ecd75a788> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/GoogleUtilities.framework/GoogleUtilities
       0x105048000 -        0x10504ffff org.cocoapods.nanopb (3.30910.0) <3a5a611f-5724-3a28-b7b9-df720d86947a> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/nanopb.framework/nanopb
       0x1081e4000 -        0x10a35ffff io.flutter.flutter (1.0) <4c4c4486-5555-3144-a1c4-573fe7e1e08b> /Users/USER/Library/Developer/CoreSimulator/Devices/2252DDC0-C915-4B0C-8C71-B97C2BC60A03/data/Containers/Bundle/Application/36717FEF-7EF1-446C-B139-C4667172DBCD/Runner.app/Frameworks/Flutter.framework/Flutter
       0x105060000 -        0x105067fff libsystem_platform.dylib (*) <93afc0a9-eec9-3f50-9339-09c7757aa50a> /usr/lib/system/libsystem_platform.dylib
       0x1054f4000 -        0x10552ffff libsystem_kernel.dylib (*) <4068b2ee-a54f-397e-882d-c5e3a40b789a> /usr/lib/system/libsystem_kernel.dylib
       0x105428000 -        0x105437fff libsystem_pthread.dylib (*) <e9238785-e581-3e65-bedb-179c698d3554> /usr/lib/system/libsystem_pthread.dylib
       0x1054cc000 -        0x1054d7fff libobjc-trampolines.dylib (*) <67028e6c-ae93-39e7-b3c8-6f6edf1cd0a5> /Volumes/VOLUME/*/libobjc-trampolines.dylib
       0x180139000 -        0x1801b62e7 libsystem_c.dylib (*) <11b4e598-e39a-34a8-9420-9a309c31374d> /Volumes/VOLUME/*/libsystem_c.dylib
       0x1802e2000 -        0x1802fa56f libc++abi.dylib (*) <1bce4456-2666-3573-a2b6-1a4e9fb5376a> /Volumes/VOLUME/*/libc++abi.dylib
       0x180070000 -        0x1800ad0d3 libobjc.A.dylib (*) <0fe5d25f-a499-3820-a943-bb603064bf8c> /Volumes/VOLUME/*/libobjc.A.dylib
       0x1803b3000 -        0x1807d175f com.apple.CoreFoundation (6.9) <189f2366-e917-3261-ba91-1c8d562f613f> /Volumes/VOLUME/*/CoreFoundation.framework/CoreFoundation
       0x185158000 -        0x18727a15f com.apple.UIKitCore (1.0) <ac67e1bc-cacf-3e1b-b45b-fe58b192b4ac> /Volumes/VOLUME/*/UIKitCore.framework/UIKitCore
       0x188485000 -        0x18855193f com.apple.FrontBoardServices (996) <d5e3a78f-ea5a-34aa-82b4-53d213d9b4d3> /Volumes/VOLUME/*/FrontBoardServices.framework/FrontBoardServices
       0x1801b7000 -        0x1801fc1bf libdispatch.dylib (*) <59a93b97-f29b-3393-8914-4559ba560b73> /Volumes/VOLUME/*/libdispatch.dylib
       0x187ee2000 -        0x187f600bf com.apple.BoardServices (1.0) <2c074346-da2b-35ae-81f1-20aeb1ddd4f9> /Volumes/VOLUME/*/BoardServices.framework/BoardServices
       0x1928cf000 -        0x1928d6dbf com.apple.GraphicsServices (1.0) <96b4e580-68f1-3d45-99c9-d40edf82691e> /Volumes/VOLUME/*/GraphicsServices.framework/GraphicsServices
               0x0 - 0xffffffffffffffff ??? (*) <00000000-0000-0000-0000-000000000000> ???
       0x1800da000 -        0x1800f7edf libsystem_trace.dylib (*) <81b58298-cefa-30ff-b54e-04d292715805> /Volumes/VOLUME/*/libsystem_trace.dylib
       0x180851000 -        0x1815bf7df com.apple.Foundation (6.9) <8cd46c12-9968-3222-864d-c654dab3d116> /Volumes/VOLUME/*/Foundation.framework/Foundation
       0x1800f8000 -        0x18013591f libxpc.dylib (*) <fff02806-1f2a-3c70-9455-959fffe4edb7> /Volumes/VOLUME/*/libxpc.dylib

EOF

-----------
Full Report
-----------

{"app_name":"Runner","timestamp":"2025-07-11 23:00:07.00 -0700","app_version":"1.0.0","slice_uuid":"4dbd5000-44a4-3f9b-930e-58f944fc5bdb","build_version":"1","platform":7,"bundleID":"com.kangengineering.universalapp.uniapp","share_with_app_devs":0,"is_first_party":0,"bug_type":"309","os_version":"macOS 15.5 (24F74)","roots_installed":0,"name":"Runner","incident_id":"70EF603D-03AD-4ECC-9532-0A3BEBD2ADE8"}
{
  "uptime" : 440000,
  "procRole" : "Foreground",
  "version" : 2,
  "userID" : 501,
  "deployVersion" : 210,
  "modelCode" : "Mac14,9",
  "coalitionID" : 65786,
  "osVersion" : {
    "train" : "macOS 15.5",
    "build" : "24F74",
    "releaseType" : "User"
  },
  "captureTime" : "2025-07-11 23:00:05.3229 -0700",
  "codeSigningMonitor" : 1,
  "incident" : "70EF603D-03AD-4ECC-9532-0A3BEBD2ADE8",
  "pid" : 97214,
  "translated" : false,
  "cpuType" : "ARM-64",
  "roots_installed" : 0,
  "bug_type" : "309",
  "procLaunch" : "2025-07-11 23:00:04.6289 -0700",
  "procStartAbsTime" : 10744267799036,
  "procExitAbsTime" : 10744282636237,
  "procName" : "Runner",
  "procPath" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Runner",
  "bundleInfo" : {"CFBundleShortVersionString":"1.0.0","CFBundleVersion":"1","CFBundleIdentifier":"com.kangengineering.universalapp.uniapp"},
  "storeInfo" : {"deviceIdentifierForVendor":"2758E48D-242F-5CED-A9B7-B4F9DD91F53E","thirdParty":true},
  "parentProc" : "launchd_sim",
  "parentPid" : 39128,
  "coalitionName" : "com.apple.CoreSimulator.SimDevice.2252DDC0-C915-4B0C-8C71-B97C2BC60A03",
  "crashReporterKey" : "D6CD3DE7-33F5-50C1-9186-F4A958BE619A",
  "appleIntelligenceStatus" : {"reasons":["notOptedIn","siriAssetIsNotReady","assetIsNotReady"],"state":"unavailable"},
  "responsiblePid" : 2442,
  "responsibleProc" : "SimulatorTrampoline",
  "codeSigningID" : "com.kangengineering.universalapp.uniapp",
  "codeSigningTeamID" : "",
  "codeSigningFlags" : 570425857,
  "codeSigningValidationCategory" : 10,
  "codeSigningTrustLevel" : 4294967295,
  "codeSigningAuxiliaryInfo" : 0,
  "instructionByteStream" : {"beforePC":"4wAAVP17v6n9AwCRIOP\/l78DAJH9e8GowANf1sADX9YQKYDSARAA1A==","atPC":"4wAAVP17v6n9AwCRFuP\/l78DAJH9e8GowANf1sADX9ZwCoDSARAA1A=="},
  "bootSessionUUID" : "AD8160D6-93FF-420E-AC78-D9DCE410585C",
  "wakeTime" : 20678,
  "sleepWakeUUID" : "593A9C95-5DF7-4BFB-B5EA-A0DD983C5420",
  "sip" : "enabled",
  "exception" : {"codes":"0x0000000000000000, 0x0000000000000000","rawCodes":[0,0],"type":"EXC_CRASH","signal":"SIGABRT"},
  "termination" : {"flags":0,"code":6,"namespace":"SIGNAL","indicator":"Abort trap: 6","byProc":"Runner","byPid":97214},
  "extMods" : {"caller":{"thread_create":0,"thread_set_state":0,"task_for_pid":0},"system":{"thread_create":0,"thread_set_state":52,"task_for_pid":4},"targeted":{"thread_create":0,"thread_set_state":0,"task_for_pid":0},"warnings":0},
  "lastExceptionBacktrace" : [{"imageOffset":1278416,"symbol":"__exceptionPreprocess","symbolLocation":160,"imageIndex":19},{"imageOffset":180100,"symbol":"objc_exception_throw","symbolLocation":72,"imageIndex":18},{"imageOffset":1278188,"symbol":"-[NSException initWithCoder:]","symbolLocation":0,"imageIndex":19},{"imageOffset":4908,"sourceLine":115,"sourceFile":"FIRApp.m","symbol":"+[FIRApp configure]","imageIndex":4,"symbolLocation":120},{"imageOffset":7444,"sourceLine":13,"sourceFile":"AppDelegate.swift","symbol":"AppDelegate.application(_:didFinishLaunchingWithOptions:)","imageIndex":2,"symbolLocation":72},{"imageOffset":8272,"sourceFile":"\/<compiler-generated>","symbol":"@objc AppDelegate.application(_:didFinishLaunchingWithOptions:)","symbolLocation":220,"imageIndex":2},{"imageOffset":17599164,"symbol":"-[UIApplication _handleDelegateCallbacksWithOptions:isSuspended:restoreState:]","symbolLocation":332,"imageIndex":20},{"imageOffset":17604600,"symbol":"-[UIApplication _callInitializationDelegatesWithActions:forScene:payload:fromOriginatingProcess:]","symbolLocation":3036,"imageIndex":20},{"imageOffset":17626168,"symbol":"-[UIApplication _runWithMainScene:transitionContext:completion:]","symbolLocation":800,"imageIndex":20},{"imageOffset":6842520,"symbol":"-[_UISceneLifecycleMultiplexer completeApplicationLaunchWithFBSScene:transitionContext:]","symbolLocation":88,"imageIndex":20},{"imageOffset":12853584,"symbol":"_UIScenePerformActionsWithLifecycleActionMask","symbolLocation":96,"imageIndex":20},{"imageOffset":6844788,"symbol":"__101-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]_block_invoke","symbolLocation":224,"imageIndex":20},{"imageOffset":6843600,"symbol":"-[_UISceneLifecycleMultiplexer _performBlock:withApplicationOfDeactivationReasons:fromReasons:]","symbolLocation":204,"imageIndex":20},{"imageOffset":6844328,"symbol":"-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]","symbolLocation":576,"imageIndex":20},{"imageOffset":6842816,"symbol":"-[_UISceneLifecycleMultiplexer uiScene:transitionedFromState:withTransitionContext:]","symbolLocation":240,"imageIndex":20},{"imageOffset":6891716,"symbol":"__186-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]_block_invoke","symbolLocation":140,"imageIndex":20},{"imageOffset":11722268,"symbol":"+[BSAnimationSettings(UIKit) tryAnimatingWithSettings:fromCurrentState:actions:completion:]","symbolLocation":656,"imageIndex":20},{"imageOffset":12953692,"symbol":"_UISceneSettingsDiffActionPerformChangesWithTransitionContextAndCompletion","symbolLocation":196,"imageIndex":20},{"imageOffset":6890960,"symbol":"-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]","symbolLocation":288,"imageIndex":20},{"imageOffset":4952148,"symbol":"__64-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]_block_invoke.190","symbolLocation":612,"imageIndex":20},{"imageOffset":4947444,"symbol":"-[UIScene _emitSceneSettingsUpdateResponseForCompletion:afterSceneUpdateWork:]","symbolLocation":200,"imageIndex":20},{"imageOffset":4951252,"symbol":"-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]","symbolLocation":220,"imageIndex":20},{"imageOffset":17621412,"symbol":"-[UIApplication workspace:didCreateScene:withTransitionContext:completion:]","symbolLocation":452,"imageIndex":20},{"imageOffset":11899884,"symbol":"-[UIApplicationSceneClientAgent scene:didInitializeWithEvent:completion:]","symbolLocation":260,"imageIndex":20},{"imageOffset":61832,"symbol":"__95-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]_block_invoke","symbolLocation":304,"imageIndex":21},{"imageOffset":62964,"symbol":"-[FBSScene _callOutQueue_maybeCoalesceClientSettingsUpdates:]","symbolLocation":116,"imageIndex":21},{"imageOffset":61404,"symbol":"-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]","symbolLocation":408,"imageIndex":21},{"imageOffset":501476,"symbol":"__93-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]_block_invoke.274","symbolLocation":232,"imageIndex":21},{"imageOffset":116268,"symbol":"-[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:]","symbolLocation":160,"imageIndex":21},{"imageOffset":239468,"symbol":"-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]","symbolLocation":392,"imageIndex":21},{"imageOffset":245312,"symbol":"__92-[FBSWorkspaceScenesClient createSceneWithIdentity:parameters:transitionContext:completion:]_block_invoke_2","symbolLocation":204,"imageIndex":21},{"imageOffset":116268,"symbol":"-[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:]","symbolLocation":160,"imageIndex":21},{"imageOffset":115888,"symbol":"_dispatch_client_callout","symbolLocation":12,"imageIndex":22},{"imageOffset":27404,"symbol":"_dispatch_block_invoke_direct","symbolLocation":376,"imageIndex":22},{"imageOffset":177980,"symbol":"__BSSERVICEMAINRUNLOOPQUEUE_IS_CALLING_OUT_TO_A_BLOCK__","symbolLocation":44,"imageIndex":23},{"imageOffset":173932,"symbol":"BSServiceMainRunLoopSourceHandler","symbolLocation":180,"imageIndex":23},{"imageOffset":600864,"symbol":"__CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__","symbolLocation":24,"imageIndex":19},{"imageOffset":600680,"symbol":"__CFRunLoopDoSource0","symbolLocation":168,"imageIndex":19},{"imageOffset":598608,"symbol":"__CFRunLoopDoSources0","symbolLocation":312,"imageIndex":19},{"imageOffset":594856,"symbol":"__CFRunLoopRun","symbolLocation":756,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":10684,"symbol":"GSEventRunModal","symbolLocation":116,"imageIndex":24},{"imageOffset":17613952,"symbol":"-[UIApplication _run]","symbolLocation":772,"imageIndex":20},{"imageOffset":17630800,"symbol":"UIApplicationMain","symbolLocation":124,"imageIndex":20},{"imageOffset":3603800,"imageIndex":20},{"imageOffset":8732,"sourceFile":"\/<compiler-generated>","symbol":"static UIApplicationDelegate.main()","symbolLocation":128,"imageIndex":2},{"imageOffset":8588,"sourceFile":"\/<compiler-generated>","symbol":"static AppDelegate.$main()","symbolLocation":44,"imageIndex":2},{"imageOffset":8856,"sourceFile":"\/<compiler-generated>","symbol":"__debug_main_executable_dylib_entry_point","symbolLocation":28,"imageIndex":2},{"imageOffset":4377842640,"imageIndex":25},{"imageOffset":27544,"symbol":"start","symbolLocation":6076,"imageIndex":0}],
  "faultingThread" : 0,
  "threads" : [{"triggered":true,"id":39610738,"threadState":{"x":[{"value":0},{"value":0},{"value":0},{"value":0},{"value":6445558955},{"value":6089745520},{"value":110},{"value":0},{"value":4381557248,"symbolLocation":0,"symbol":"_main_thread"},{"value":3839969546405957164},{"value":81},{"value":11},{"value":11},{"value":6449838836},{"value":2043},{"value":2596489228},{"value":328},{"value":2598584337},{"value":0},{"value":6},{"value":259},{"value":4381557472,"symbolLocation":224,"symbol":"_main_thread"},{"value":8368631808,"symbolLocation":0,"symbol":"LazyClassNamerHook"},{"value":0},{"value":0},{"value":8370827264,"symbolLocation":16,"symbol":"OBJC_CLASS_$_UIVisualEffectBackingHost"},{"value":8370544640,"symbolLocation":12,"symbol":"_MergedGlobals"},{"value":730267748},{"value":16}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383236844},"cpsr":{"value":1073745920},"fp":{"value":6089745376},"sp":{"value":6089745344},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384082036,"matchesCrashFrame":1},"far":{"value":0}},"queue":"com.apple.main-thread","frames":[{"imageOffset":34932,"symbol":"__pthread_kill","symbolLocation":8,"imageIndex":13},{"imageOffset":25324,"symbol":"pthread_kill","symbolLocation":264,"imageIndex":14},{"imageOffset":477624,"symbol":"abort","symbolLocation":100,"imageIndex":16},{"imageOffset":70252,"symbol":"__abort_message","symbolLocation":128,"imageIndex":17},{"imageOffset":4516,"symbol":"demangling_terminate_handler()","symbolLocation":268,"imageIndex":17},{"imageOffset":29208,"symbol":"_objc_terminate()","symbolLocation":124,"imageIndex":18},{"imageOffset":67416,"symbol":"std::__terminate(void (*)())","symbolLocation":12,"imageIndex":17},{"imageOffset":79808,"symbol":"__cxxabiv1::failed_throw(__cxxabiv1::__cxa_exception*)","symbolLocation":32,"imageIndex":17},{"imageOffset":79776,"symbol":"__cxa_throw","symbolLocation":88,"imageIndex":17},{"imageOffset":180412,"symbol":"objc_exception_throw","symbolLocation":384,"imageIndex":18},{"imageOffset":1278188,"symbol":"+[NSException raise:format:]","symbolLocation":124,"imageIndex":19},{"imageOffset":4908,"sourceLine":110,"sourceFile":"FIRApp.m","symbol":"+[FIRApp configure]","imageIndex":4,"symbolLocation":120},{"imageOffset":7444,"sourceLine":12,"sourceFile":"AppDelegate.swift","symbol":"AppDelegate.application(_:didFinishLaunchingWithOptions:)","imageIndex":2,"symbolLocation":72},{"imageOffset":8272,"sourceFile":"\/<compiler-generated>","symbol":"@objc AppDelegate.application(_:didFinishLaunchingWithOptions:)","symbolLocation":220,"imageIndex":2},{"imageOffset":17599164,"symbol":"-[UIApplication _handleDelegateCallbacksWithOptions:isSuspended:restoreState:]","symbolLocation":332,"imageIndex":20},{"imageOffset":17604600,"symbol":"-[UIApplication _callInitializationDelegatesWithActions:forScene:payload:fromOriginatingProcess:]","symbolLocation":3036,"imageIndex":20},{"imageOffset":17626168,"symbol":"-[UIApplication _runWithMainScene:transitionContext:completion:]","symbolLocation":800,"imageIndex":20},{"imageOffset":6842520,"symbol":"-[_UISceneLifecycleMultiplexer completeApplicationLaunchWithFBSScene:transitionContext:]","symbolLocation":88,"imageIndex":20},{"imageOffset":12853584,"symbol":"_UIScenePerformActionsWithLifecycleActionMask","symbolLocation":96,"imageIndex":20},{"imageOffset":6844788,"symbol":"__101-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]_block_invoke","symbolLocation":224,"imageIndex":20},{"imageOffset":6843600,"symbol":"-[_UISceneLifecycleMultiplexer _performBlock:withApplicationOfDeactivationReasons:fromReasons:]","symbolLocation":204,"imageIndex":20},{"imageOffset":6844328,"symbol":"-[_UISceneLifecycleMultiplexer _evalTransitionToSettings:fromSettings:forceExit:withTransitionStore:]","symbolLocation":576,"imageIndex":20},{"imageOffset":6842816,"symbol":"-[_UISceneLifecycleMultiplexer uiScene:transitionedFromState:withTransitionContext:]","symbolLocation":240,"imageIndex":20},{"imageOffset":6891716,"symbol":"__186-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]_block_invoke","symbolLocation":140,"imageIndex":20},{"imageOffset":11722268,"symbol":"+[BSAnimationSettings(UIKit) tryAnimatingWithSettings:fromCurrentState:actions:completion:]","symbolLocation":656,"imageIndex":20},{"imageOffset":12953692,"symbol":"_UISceneSettingsDiffActionPerformChangesWithTransitionContextAndCompletion","symbolLocation":196,"imageIndex":20},{"imageOffset":6890960,"symbol":"-[_UIWindowSceneFBSSceneTransitionContextDrivenLifecycleSettingsDiffAction _performActionsForUIScene:withUpdatedFBSScene:settingsDiff:fromSettings:transitionContext:lifecycleActionType:]","symbolLocation":288,"imageIndex":20},{"imageOffset":4952148,"symbol":"__64-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]_block_invoke.190","symbolLocation":612,"imageIndex":20},{"imageOffset":4947444,"symbol":"-[UIScene _emitSceneSettingsUpdateResponseForCompletion:afterSceneUpdateWork:]","symbolLocation":200,"imageIndex":20},{"imageOffset":4951252,"symbol":"-[UIScene scene:didUpdateWithDiff:transitionContext:completion:]","symbolLocation":220,"imageIndex":20},{"imageOffset":17621412,"symbol":"-[UIApplication workspace:didCreateScene:withTransitionContext:completion:]","symbolLocation":452,"imageIndex":20},{"imageOffset":11899884,"symbol":"-[UIApplicationSceneClientAgent scene:didInitializeWithEvent:completion:]","symbolLocation":260,"imageIndex":20},{"imageOffset":61832,"symbol":"__95-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]_block_invoke","symbolLocation":304,"imageIndex":21},{"imageOffset":62964,"symbol":"-[FBSScene _callOutQueue_maybeCoalesceClientSettingsUpdates:]","symbolLocation":116,"imageIndex":21},{"imageOffset":61404,"symbol":"-[FBSScene _callOutQueue_didCreateWithTransitionContext:alternativeCreationCallout:completion:]","symbolLocation":408,"imageIndex":21},{"imageOffset":501476,"symbol":"__93-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]_block_invoke.274","symbolLocation":232,"imageIndex":21},{"imageOffset":116268,"symbol":"-[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:]","symbolLocation":160,"imageIndex":21},{"imageOffset":239468,"symbol":"-[FBSWorkspaceScenesClient _callOutQueue_sendDidCreateForScene:transitionContext:completion:]","symbolLocation":392,"imageIndex":21},{"imageOffset":245312,"symbol":"__92-[FBSWorkspaceScenesClient createSceneWithIdentity:parameters:transitionContext:completion:]_block_invoke_2","symbolLocation":204,"imageIndex":21},{"imageOffset":116268,"symbol":"-[FBSWorkspace _calloutQueue_executeCalloutFromSource:withBlock:]","symbolLocation":160,"imageIndex":21},{"imageOffset":115888,"symbol":"_dispatch_client_callout","symbolLocation":12,"imageIndex":22},{"imageOffset":27404,"symbol":"_dispatch_block_invoke_direct","symbolLocation":376,"imageIndex":22},{"imageOffset":177980,"symbol":"__BSSERVICEMAINRUNLOOPQUEUE_IS_CALLING_OUT_TO_A_BLOCK__","symbolLocation":44,"imageIndex":23},{"imageOffset":173932,"symbol":"BSServiceMainRunLoopSourceHandler","symbolLocation":180,"imageIndex":23},{"imageOffset":600864,"symbol":"__CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE0_PERFORM_FUNCTION__","symbolLocation":24,"imageIndex":19},{"imageOffset":600680,"symbol":"__CFRunLoopDoSource0","symbolLocation":168,"imageIndex":19},{"imageOffset":598608,"symbol":"__CFRunLoopDoSources0","symbolLocation":312,"imageIndex":19},{"imageOffset":594856,"symbol":"__CFRunLoopRun","symbolLocation":756,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":10684,"symbol":"GSEventRunModal","symbolLocation":116,"imageIndex":24},{"imageOffset":17613952,"symbol":"-[UIApplication _run]","symbolLocation":772,"imageIndex":20},{"imageOffset":17630800,"symbol":"UIApplicationMain","symbolLocation":124,"imageIndex":20},{"imageOffset":3603800,"imageIndex":20},{"imageOffset":8732,"sourceFile":"\/<compiler-generated>","symbol":"static UIApplicationDelegate.main()","symbolLocation":128,"imageIndex":2},{"imageOffset":8588,"sourceFile":"\/<compiler-generated>","symbol":"static AppDelegate.$main()","symbolLocation":44,"imageIndex":2},{"imageOffset":8856,"sourceFile":"\/<compiler-generated>","symbol":"__debug_main_executable_dylib_entry_point","symbolLocation":28,"imageIndex":2},{"imageOffset":4377842640,"imageIndex":25},{"imageOffset":27544,"symbol":"start","symbolLocation":6076,"imageIndex":0}]},{"id":39610798,"frames":[{"imageOffset":6532,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":14}],"threadState":{"x":[{"value":6090321920},{"value":2307},{"value":6089785344},{"value":0},{"value":409604},{"value":18446744073709551615},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":0},"cpsr":{"value":4096},"fp":{"value":0},"sp":{"value":6090321920},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4383218052},"far":{"value":0}}},{"id":39610799,"threadState":{"x":[{"value":18446744073709551612},{"value":0},{"value":4294967295},{"value":0},{"value":8368621696,"symbolLocation":0,"symbol":"_dispatch_main_q"},{"value":18},{"value":0},{"value":0},{"value":0},{"value":6},{"value":105553140565062},{"value":105553140565072},{"value":8368621800,"symbolLocation":104,"symbol":"_dispatch_main_q"},{"value":8368621744,"symbolLocation":48,"symbol":"_dispatch_main_q"},{"value":9005068950962176},{"value":9005137670438912},{"value":515},{"value":2554726465},{"value":0},{"value":4294967295},{"value":1},{"value":0},{"value":6090893056},{"value":8368621696,"symbolLocation":0,"symbol":"_dispatch_main_q"},{"value":18},{"value":6527746048},{"value":0},{"value":0},{"value":9223372036891514386}],"flavor":"ARM_THREAD_STATE64","lr":{"value":6444262832},"cpsr":{"value":1073745920},"fp":{"value":6090892864},"sp":{"value":6090892832},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384057200},"far":{"value":0}},"queue":"com.apple.libtrace.state.block-list","frames":[{"imageOffset":10096,"symbol":"__ulock_wait","symbolLocation":8,"imageIndex":13},{"imageOffset":13744,"symbol":"_dlock_wait","symbolLocation":52,"imageIndex":22},{"imageOffset":13244,"symbol":"_dispatch_thread_event_wait_slow","symbolLocation":52,"imageIndex":22},{"imageOffset":74600,"symbol":"__DISPATCH_WAIT_FOR_QUEUE__","symbolLocation":392,"imageIndex":22},{"imageOffset":73316,"symbol":"_dispatch_sync_f_slow","symbolLocation":160,"imageIndex":22},{"imageOffset":102288,"symbol":"___os_state_request_for_self_block_invoke","symbolLocation":340,"imageIndex":26},{"imageOffset":6056,"symbol":"_dispatch_call_block_and_release","symbolLocation":24,"imageIndex":22},{"imageOffset":115888,"symbol":"_dispatch_client_callout","symbolLocation":12,"imageIndex":22},{"imageOffset":44072,"symbol":"_dispatch_lane_serial_drain","symbolLocation":984,"imageIndex":22},{"imageOffset":46824,"symbol":"_dispatch_lane_invoke","symbolLocation":396,"imageIndex":22},{"imageOffset":91444,"symbol":"_dispatch_root_queue_drain_deferred_wlh","symbolLocation":288,"imageIndex":22},{"imageOffset":89204,"symbol":"_dispatch_workloop_worker_thread","symbolLocation":692,"imageIndex":22},{"imageOffset":11212,"symbol":"_pthread_wqthread","symbolLocation":288,"imageIndex":14},{"imageOffset":6540,"symbol":"start_wqthread","symbolLocation":8,"imageIndex":14}]},{"id":39610804,"threadState":{"x":[{"value":18446744073709551612},{"value":0},{"value":4294967295},{"value":0},{"value":8368621696,"symbolLocation":0,"symbol":"_dispatch_main_q"},{"value":18},{"value":0},{"value":0},{"value":0},{"value":6},{"value":6090892966},{"value":6090892976},{"value":8368621800,"symbolLocation":104,"symbol":"_dispatch_main_q"},{"value":8368621744,"symbolLocation":48,"symbol":"_dispatch_main_q"},{"value":9005068950962176},{"value":8368818864,"symbolLocation":0,"symbol":"OBJC_CLASS_$_NSMethodSignature"},{"value":515},{"value":288230384522794313,"symbolLocation":288230376151711745,"symbol":"OBJC_CLASS_$__UIKeyboardChangedInformation"},{"value":0},{"value":4294967295},{"value":1},{"value":0},{"value":6091464400},{"value":8368621696,"symbolLocation":0,"symbol":"_dispatch_main_q"},{"value":18},{"value":2148468479},{"value":4351},{"value":8447},{"value":105553140438592}],"flavor":"ARM_THREAD_STATE64","lr":{"value":6444262832},"cpsr":{"value":1073745920},"fp":{"value":6091464208},"sp":{"value":6091464176},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384057200},"far":{"value":0}},"queue":"com.apple.UIKit.KeyboardManagement","frames":[{"imageOffset":10096,"symbol":"__ulock_wait","symbolLocation":8,"imageIndex":13},{"imageOffset":13744,"symbol":"_dlock_wait","symbolLocation":52,"imageIndex":22},{"imageOffset":13244,"symbol":"_dispatch_thread_event_wait_slow","symbolLocation":52,"imageIndex":22},{"imageOffset":74600,"symbol":"__DISPATCH_WAIT_FOR_QUEUE__","symbolLocation":392,"imageIndex":22},{"imageOffset":73316,"symbol":"_dispatch_sync_f_slow","symbolLocation":160,"imageIndex":22},{"imageOffset":15776148,"symbol":"__37-[_UIRemoteKeyboards startConnection]_block_invoke.388","symbolLocation":116,"imageIndex":20},{"imageOffset":1305504,"symbol":"__invoking___","symbolLocation":144,"imageIndex":19},{"imageOffset":1293648,"symbol":"-[NSInvocation invoke]","symbolLocation":276,"imageIndex":19},{"imageOffset":9989216,"symbol":"<deduplicated_symbol>","symbolLocation":12,"imageIndex":27},{"imageOffset":9988300,"symbol":"-[NSXPCConnection _decodeAndInvokeReplyBlockWithEvent:sequence:replyInfo:]","symbolLocation":484,"imageIndex":27},{"imageOffset":10004404,"symbol":"__88-[NSXPCConnection _sendInvocation:orArguments:count:methodSignature:selector:withProxy:]_block_invoke_5","symbolLocation":184,"imageIndex":27},{"imageOffset":117028,"symbol":"_xpc_connection_reply_callout","symbolLocation":60,"imageIndex":28},{"imageOffset":63676,"symbol":"_xpc_connection_call_reply_async","symbolLocation":92,"imageIndex":28},{"imageOffset":115928,"symbol":"<deduplicated_symbol>","symbolLocation":12,"imageIndex":22},{"imageOffset":134148,"symbol":"_dispatch_mach_msg_async_reply_invoke","symbolLocation":508,"imageIndex":22},{"imageOffset":43392,"symbol":"_dispatch_lane_serial_drain","symbolLocation":304,"imageIndex":22},{"imageOffset":46824,"symbol":"_dispatch_lane_invoke","symbolLocation":396,"imageIndex":22},{"imageOffset":91444,"symbol":"_dispatch_root_queue_drain_deferred_wlh","symbolLocation":288,"imageIndex":22},{"imageOffset":89204,"symbol":"_dispatch_workloop_worker_thread","symbolLocation":692,"imageIndex":22},{"imageOffset":11212,"symbol":"_pthread_wqthread","symbolLocation":288,"imageIndex":14},{"imageOffset":6540,"symbol":"start_wqthread","symbolLocation":8,"imageIndex":14}]},{"id":39610806,"frames":[{"imageOffset":6532,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":14}],"threadState":{"x":[{"value":6092042240},{"value":9731},{"value":6091505664},{"value":0},{"value":409602},{"value":18446744073709551615},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":0},"cpsr":{"value":4096},"fp":{"value":0},"sp":{"value":6092042240},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4383218052},"far":{"value":0}}},{"id":39610807,"name":"com.apple.uikit.eventfetch-thread","threadState":{"x":[{"value":268451845},{"value":21592279046},{"value":8589934592},{"value":51689931407360},{"value":2162692},{"value":51689931407360},{"value":2},{"value":4294967295},{"value":0},{"value":17179869184},{"value":0},{"value":2},{"value":0},{"value":0},{"value":12035},{"value":3072},{"value":18446744073709551569},{"value":2156130299},{"value":0},{"value":4294967295},{"value":2},{"value":51689931407360},{"value":2162692},{"value":51689931407360},{"value":6092610952},{"value":8589934592},{"value":21592279046},{"value":18446744073709550527},{"value":4412409862}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4384120748},"cpsr":{"value":4096},"fp":{"value":6092610800},"sp":{"value":6092610720},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384050032},"far":{"value":0}},"frames":[{"imageOffset":2928,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":13},{"imageOffset":73644,"symbol":"mach_msg2_internal","symbolLocation":72,"imageIndex":13},{"imageOffset":35880,"symbol":"mach_msg_overwrite","symbolLocation":480,"imageIndex":13},{"imageOffset":3800,"symbol":"mach_msg","symbolLocation":20,"imageIndex":13},{"imageOffset":598912,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":156,"imageIndex":19},{"imageOffset":595220,"symbol":"__CFRunLoopRun","symbolLocation":1120,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":9054176,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":208,"imageIndex":27},{"imageOffset":9054720,"symbol":"-[NSRunLoop(NSRunLoop) runUntilDate:]","symbolLocation":60,"imageIndex":27},{"imageOffset":18362372,"symbol":"-[UIEventFetcher threadMain]","symbolLocation":408,"imageIndex":20},{"imageOffset":9213652,"symbol":"__NSThread__start__","symbolLocation":716,"imageIndex":27},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610817,"name":"io.flutter.1.raster","threadState":{"x":[{"value":268451845},{"value":21592279046},{"value":8589934592},{"value":101167954657280},{"value":0},{"value":101167954657280},{"value":2},{"value":4294967295},{"value":0},{"value":17179869184},{"value":0},{"value":2},{"value":0},{"value":0},{"value":23555},{"value":3072},{"value":18446744073709551569},{"value":2},{"value":0},{"value":4294967295},{"value":2},{"value":101167954657280},{"value":0},{"value":101167954657280},{"value":6094757896},{"value":8589934592},{"value":21592279046},{"value":18446744073709550527},{"value":4412409862}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4384120748},"cpsr":{"value":4096},"fp":{"value":6094757744},"sp":{"value":6094757664},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384050032},"far":{"value":0}},"frames":[{"imageOffset":2928,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":13},{"imageOffset":73644,"symbol":"mach_msg2_internal","symbolLocation":72,"imageIndex":13},{"imageOffset":35880,"symbol":"mach_msg_overwrite","symbolLocation":480,"imageIndex":13},{"imageOffset":3800,"symbol":"mach_msg","symbolLocation":20,"imageIndex":13},{"imageOffset":598912,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":156,"imageIndex":19},{"imageOffset":595220,"symbol":"__CFRunLoopRun","symbolLocation":1120,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":582712,"symbol":"fml::MessageLoopDarwin::Run()","symbolLocation":88,"imageIndex":11},{"imageOffset":555012,"symbol":"fml::MessageLoopImpl::DoRun()","symbolLocation":40,"imageIndex":11},{"imageOffset":577744,"symbol":"std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()()","symbolLocation":184,"imageIndex":11},{"imageOffset":576932,"symbol":"fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*)","symbolLocation":36,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610818,"name":"io.flutter.1.io","threadState":{"x":[{"value":268451845},{"value":21592279046},{"value":8589934592},{"value":108864536051712},{"value":0},{"value":108864536051712},{"value":2},{"value":4294967295},{"value":0},{"value":17179869184},{"value":0},{"value":2},{"value":0},{"value":0},{"value":25347},{"value":3072},{"value":18446744073709551569},{"value":2},{"value":0},{"value":4294967295},{"value":2},{"value":108864536051712},{"value":0},{"value":108864536051712},{"value":6096904200},{"value":8589934592},{"value":21592279046},{"value":18446744073709550527},{"value":4412409862}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4384120748},"cpsr":{"value":4096},"fp":{"value":6096904048},"sp":{"value":6096903968},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384050032},"far":{"value":0}},"frames":[{"imageOffset":2928,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":13},{"imageOffset":73644,"symbol":"mach_msg2_internal","symbolLocation":72,"imageIndex":13},{"imageOffset":35880,"symbol":"mach_msg_overwrite","symbolLocation":480,"imageIndex":13},{"imageOffset":3800,"symbol":"mach_msg","symbolLocation":20,"imageIndex":13},{"imageOffset":598912,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":156,"imageIndex":19},{"imageOffset":595220,"symbol":"__CFRunLoopRun","symbolLocation":1120,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":582712,"symbol":"fml::MessageLoopDarwin::Run()","symbolLocation":88,"imageIndex":11},{"imageOffset":555012,"symbol":"fml::MessageLoopImpl::DoRun()","symbolLocation":40,"imageIndex":11},{"imageOffset":577744,"symbol":"std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()()","symbolLocation":184,"imageIndex":11},{"imageOffset":576932,"symbol":"fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*)","symbolLocation":36,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610819,"name":"io.flutter.1.profiler","threadState":{"x":[{"value":268451845},{"value":21592279046},{"value":8589934592},{"value":114362094190592},{"value":0},{"value":114362094190592},{"value":2},{"value":4294967295},{"value":0},{"value":17179869184},{"value":0},{"value":2},{"value":0},{"value":0},{"value":26627},{"value":3072},{"value":18446744073709551569},{"value":2},{"value":0},{"value":4294967295},{"value":2},{"value":114362094190592},{"value":0},{"value":114362094190592},{"value":6099050504},{"value":8589934592},{"value":21592279046},{"value":18446744073709550527},{"value":4412409862}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4384120748},"cpsr":{"value":4096},"fp":{"value":6099050352},"sp":{"value":6099050272},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384050032},"far":{"value":0}},"frames":[{"imageOffset":2928,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":13},{"imageOffset":73644,"symbol":"mach_msg2_internal","symbolLocation":72,"imageIndex":13},{"imageOffset":35880,"symbol":"mach_msg_overwrite","symbolLocation":480,"imageIndex":13},{"imageOffset":3800,"symbol":"mach_msg","symbolLocation":20,"imageIndex":13},{"imageOffset":598912,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":156,"imageIndex":19},{"imageOffset":595220,"symbol":"__CFRunLoopRun","symbolLocation":1120,"imageIndex":19},{"imageOffset":574552,"symbol":"_CFRunLoopRunSpecificWithOptions","symbolLocation":496,"imageIndex":19},{"imageOffset":582712,"symbol":"fml::MessageLoopDarwin::Run()","symbolLocation":88,"imageIndex":11},{"imageOffset":555012,"symbol":"fml::MessageLoopImpl::DoRun()","symbolLocation":40,"imageIndex":11},{"imageOffset":577744,"symbol":"std::_fl::__function::__func<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0, std::_fl::allocator<fml::Thread::Thread(std::_fl::function<void (fml::Thread::ThreadConfig const&)> const&, fml::Thread::ThreadConfig const&)::$_0>, void ()>::operator()()","symbolLocation":184,"imageIndex":11},{"imageOffset":576932,"symbol":"fml::ThreadHandle::ThreadHandle(std::_fl::function<void ()>&&)::$_0::__invoke(void*)","symbolLocation":36,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610820,"name":"io.worker.1","threadState":{"x":[{"value":4},{"value":0},{"value":1024},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6099627480},{"value":0},{"value":512},{"value":2199023256066},{"value":2199023256066},{"value":512},{"value":0},{"value":2199023256064},{"value":305},{"value":83},{"value":0},{"value":4429222904},{"value":4429222968},{"value":6099628256},{"value":0},{"value":0},{"value":1024},{"value":1025},{"value":1280},{"value":1},{"value":105553118562912}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238840},"cpsr":{"value":1610616832},"fp":{"value":6099627600},"sp":{"value":6099627456},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27320,"symbol":"_pthread_cond_wait","symbolLocation":976,"imageIndex":14},{"imageOffset":411992,"symbol":"std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&)","symbolLocation":24,"imageIndex":11},{"imageOffset":540212,"symbol":"fml::ConcurrentMessageLoop::WorkerMain()","symbolLocation":140,"imageIndex":11},{"imageOffset":542560,"symbol":"void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*)","symbolLocation":212,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610821,"name":"io.worker.2","threadState":{"x":[{"value":4},{"value":0},{"value":1024},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6100200920},{"value":0},{"value":512},{"value":2199023256066},{"value":2199023256066},{"value":512},{"value":0},{"value":2199023256064},{"value":305},{"value":84},{"value":0},{"value":4429222904},{"value":4429222968},{"value":6100201696},{"value":0},{"value":0},{"value":1024},{"value":1024},{"value":1536},{"value":1},{"value":105553118562944}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238840},"cpsr":{"value":1610616832},"fp":{"value":6100201040},"sp":{"value":6100200896},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27320,"symbol":"_pthread_cond_wait","symbolLocation":976,"imageIndex":14},{"imageOffset":411992,"symbol":"std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&)","symbolLocation":24,"imageIndex":11},{"imageOffset":540212,"symbol":"fml::ConcurrentMessageLoop::WorkerMain()","symbolLocation":140,"imageIndex":11},{"imageOffset":542560,"symbol":"void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*)","symbolLocation":212,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610822,"name":"io.worker.3","threadState":{"x":[{"value":4},{"value":0},{"value":1024},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6100774360},{"value":0},{"value":512},{"value":2199023256066},{"value":2199023256066},{"value":512},{"value":0},{"value":2199023256064},{"value":305},{"value":85},{"value":0},{"value":4429222904},{"value":4429222968},{"value":6100775136},{"value":0},{"value":0},{"value":1024},{"value":1024},{"value":2048},{"value":1},{"value":105553118562976}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238840},"cpsr":{"value":1610616832},"fp":{"value":6100774480},"sp":{"value":6100774336},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27320,"symbol":"_pthread_cond_wait","symbolLocation":976,"imageIndex":14},{"imageOffset":411992,"symbol":"std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&)","symbolLocation":24,"imageIndex":11},{"imageOffset":540212,"symbol":"fml::ConcurrentMessageLoop::WorkerMain()","symbolLocation":140,"imageIndex":11},{"imageOffset":542560,"symbol":"void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*)","symbolLocation":212,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610823,"name":"io.worker.4","threadState":{"x":[{"value":260},{"value":0},{"value":1024},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6101347800},{"value":0},{"value":512},{"value":2199023256066},{"value":2199023256066},{"value":512},{"value":0},{"value":2199023256064},{"value":305},{"value":86},{"value":0},{"value":4429222904},{"value":4429222968},{"value":6101348576},{"value":0},{"value":0},{"value":1024},{"value":1024},{"value":1792},{"value":1},{"value":105553118563008}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238840},"cpsr":{"value":1610616832},"fp":{"value":6101347920},"sp":{"value":6101347776},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27320,"symbol":"_pthread_cond_wait","symbolLocation":976,"imageIndex":14},{"imageOffset":411992,"symbol":"std::_fl::condition_variable::wait(std::_fl::unique_lock<std::_fl::mutex>&)","symbolLocation":24,"imageIndex":11},{"imageOffset":540212,"symbol":"fml::ConcurrentMessageLoop::WorkerMain()","symbolLocation":140,"imageIndex":11},{"imageOffset":542560,"symbol":"void* std::_fl::__thread_proxy[abi:nn210000]<std::_fl::tuple<std::_fl::unique_ptr<std::_fl::__thread_struct, std::_fl::default_delete<std::_fl::__thread_struct>>, fml::ConcurrentMessageLoop::ConcurrentMessageLoop(unsigned long)::$_0>>(void*)","symbolLocation":212,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610824,"name":"dart:io EventHandler","threadState":{"x":[{"value":4},{"value":0},{"value":0},{"value":6102445336},{"value":16},{"value":6102444296},{"value":105553118514560},{"value":0},{"value":998000000},{"value":119},{"value":244838346588160},{"value":32},{"value":105553116268808},{"value":2095104},{"value":2043},{"value":3985184877},{"value":363},{"value":3987279921},{"value":0},{"value":105553156181376},{"value":6102444296},{"value":67108864},{"value":2147483647},{"value":274877907},{"value":4294966296},{"value":1000000},{"value":610073207},{"value":0},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4436221432},"cpsr":{"value":536875008},"fp":{"value":6102445936},"sp":{"value":6102444272},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384073328},"far":{"value":0}},"frames":[{"imageOffset":26224,"symbol":"kevent","symbolLocation":8,"imageIndex":13},{"imageOffset":5053944,"symbol":"dart::bin::EventHandlerImplementation::EventHandlerEntry(unsigned long)","symbolLocation":300,"imageIndex":11},{"imageOffset":5168976,"symbol":"dart::bin::ThreadStart(void*)","symbolLocation":88,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610825,"name":"Dart Profiler ThreadInterrupter","threadState":{"x":[{"value":260},{"value":0},{"value":256},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6103542296},{"value":0},{"value":0},{"value":2},{"value":2},{"value":0},{"value":0},{"value":0},{"value":305},{"value":50577534889728},{"value":0},{"value":105553162483200},{"value":105553162483272},{"value":6103544032},{"value":0},{"value":0},{"value":256},{"value":12033},{"value":12288},{"value":4467036160,"symbolLocation":3816,"symbol":"dart::Symbols::symbol_handles_"},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238840},"cpsr":{"value":1610616832},"fp":{"value":6103542416},"sp":{"value":6103542272},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27320,"symbol":"_pthread_cond_wait","symbolLocation":976,"imageIndex":14},{"imageOffset":5477976,"symbol":"dart::ConditionVariable::WaitMicros(dart::Mutex*, long long)","symbolLocation":128,"imageIndex":11},{"imageOffset":6907380,"symbol":"dart::ThreadInterrupter::ThreadMain(unsigned long)","symbolLocation":328,"imageIndex":11},{"imageOffset":6610980,"symbol":"dart::ThreadStart(void*)","symbolLocation":204,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610826,"name":"Dart Profiler SampleBlockProcessor","threadState":{"x":[{"value":260},{"value":0},{"value":256},{"value":0},{"value":0},{"value":160},{"value":0},{"value":100000000},{"value":257},{"value":0},{"value":0},{"value":2},{"value":2},{"value":0},{"value":0},{"value":0},{"value":305},{"value":256},{"value":0},{"value":105553162483328},{"value":105553162483400},{"value":1},{"value":100000000},{"value":0},{"value":256},{"value":257},{"value":512},{"value":0},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238884},"cpsr":{"value":2684358656},"fp":{"value":6104640144},"sp":{"value":6104640000},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27364,"symbol":"_pthread_cond_wait","symbolLocation":1020,"imageIndex":14},{"imageOffset":5477960,"symbol":"dart::ConditionVariable::WaitMicros(dart::Mutex*, long long)","symbolLocation":112,"imageIndex":11},{"imageOffset":6630128,"symbol":"dart::SampleBlockProcessor::ThreadMain(unsigned long)","symbolLocation":168,"imageIndex":11},{"imageOffset":6610980,"symbol":"dart::ThreadStart(void*)","symbolLocation":204,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610827,"name":"DartWorker","threadState":{"x":[{"value":260},{"value":0},{"value":0},{"value":0},{"value":0},{"value":160},{"value":5},{"value":0},{"value":1},{"value":0},{"value":0},{"value":2},{"value":2},{"value":0},{"value":0},{"value":0},{"value":305},{"value":82},{"value":0},{"value":4429227112},{"value":105553156182960},{"value":1},{"value":0},{"value":5},{"value":0},{"value":1},{"value":256},{"value":4467036160,"symbolLocation":3816,"symbol":"dart::Symbols::symbol_handles_"},{"value":1000}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238884},"cpsr":{"value":2684358656},"fp":{"value":6105737792},"sp":{"value":6105737648},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27364,"symbol":"_pthread_cond_wait","symbolLocation":1020,"imageIndex":14},{"imageOffset":5477960,"symbol":"dart::ConditionVariable::WaitMicros(dart::Mutex*, long long)","symbolLocation":112,"imageIndex":11},{"imageOffset":6910828,"symbol":"dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*)","symbolLocation":508,"imageIndex":11},{"imageOffset":6911172,"symbol":"dart::ThreadPool::Worker::Main(unsigned long)","symbolLocation":116,"imageIndex":11},{"imageOffset":6610980,"symbol":"dart::ThreadStart(void*)","symbolLocation":204,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610829,"frames":[{"imageOffset":6532,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":14}],"threadState":{"x":[{"value":6106312704},{"value":33799},{"value":6105776128},{"value":0},{"value":409604},{"value":18446744073709551615},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0},{"value":0}],"flavor":"ARM_THREAD_STATE64","lr":{"value":0},"cpsr":{"value":4096},"fp":{"value":0},"sp":{"value":6106312704},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4383218052},"far":{"value":0}}},{"id":39610831,"name":"DartWorker","threadState":{"x":[{"value":260},{"value":0},{"value":0},{"value":0},{"value":0},{"value":160},{"value":5},{"value":0},{"value":1},{"value":0},{"value":0},{"value":2},{"value":2},{"value":0},{"value":0},{"value":0},{"value":305},{"value":287},{"value":0},{"value":4429236632},{"value":105553156182672},{"value":1},{"value":0},{"value":5},{"value":0},{"value":1},{"value":256},{"value":4467036160,"symbolLocation":3816,"symbol":"dart::Symbols::symbol_handles_"},{"value":1000}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238884},"cpsr":{"value":2684358656},"fp":{"value":6107408960},"sp":{"value":6107408816},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27364,"symbol":"_pthread_cond_wait","symbolLocation":1020,"imageIndex":14},{"imageOffset":5477960,"symbol":"dart::ConditionVariable::WaitMicros(dart::Mutex*, long long)","symbolLocation":112,"imageIndex":11},{"imageOffset":6910828,"symbol":"dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*)","symbolLocation":508,"imageIndex":11},{"imageOffset":6911172,"symbol":"dart::ThreadPool::Worker::Main(unsigned long)","symbolLocation":116,"imageIndex":11},{"imageOffset":6610980,"symbol":"dart::ThreadStart(void*)","symbolLocation":204,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]},{"id":39610832,"name":"DartWorker","threadState":{"x":[{"value":260},{"value":0},{"value":0},{"value":0},{"value":0},{"value":160},{"value":61},{"value":0},{"value":1},{"value":0},{"value":0},{"value":2},{"value":2},{"value":0},{"value":0},{"value":0},{"value":305},{"value":27},{"value":0},{"value":4480591720},{"value":105553156234704},{"value":1},{"value":0},{"value":61},{"value":0},{"value":1},{"value":256},{"value":4467036160,"symbolLocation":3816,"symbol":"dart::Symbols::symbol_handles_"},{"value":1000}],"flavor":"ARM_THREAD_STATE64","lr":{"value":4383238884},"cpsr":{"value":2684358656},"fp":{"value":6108506608},"sp":{"value":6108506464},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":4384063508},"far":{"value":0}},"frames":[{"imageOffset":16404,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":13},{"imageOffset":27364,"symbol":"_pthread_cond_wait","symbolLocation":1020,"imageIndex":14},{"imageOffset":5477960,"symbol":"dart::ConditionVariable::WaitMicros(dart::Mutex*, long long)","symbolLocation":112,"imageIndex":11},{"imageOffset":5863564,"symbol":"dart::MutatorThreadPool::OnEnterIdleLocked(dart::MutexLocker*, dart::ThreadPool::Worker*)","symbolLocation":152,"imageIndex":11},{"imageOffset":6910444,"symbol":"dart::ThreadPool::WorkerLoop(dart::ThreadPool::Worker*)","symbolLocation":124,"imageIndex":11},{"imageOffset":6911172,"symbol":"dart::ThreadPool::Worker::Main(unsigned long)","symbolLocation":116,"imageIndex":11},{"imageOffset":6610980,"symbol":"dart::ThreadStart(void*)","symbolLocation":204,"imageIndex":11},{"imageOffset":26096,"symbol":"_pthread_start","symbolLocation":104,"imageIndex":14},{"imageOffset":6552,"symbol":"thread_start","symbolLocation":8,"imageIndex":14}]}],
  "usedImages" : [
  {
    "source" : "P",
    "arch" : "arm64e",
    "base" : 4380868608,
    "size" : 638976,
    "uuid" : "9cf0401a-a938-389e-a77d-9e9608076ccf",
    "path" : "\/usr\/lib\/dyld",
    "name" : "dyld"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4377116672,
    "CFBundleShortVersionString" : "1.0.0",
    "CFBundleIdentifier" : "com.kangengineering.universalapp.uniapp",
    "size" : 16384,
    "uuid" : "4dbd5000-44a4-3f9b-930e-58f944fc5bdb",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Runner",
    "name" : "Runner",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4377493504,
    "size" : 131072,
    "uuid" : "e8a0ad9f-a387-3e8a-ac25-aaac11c07124",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Runner.debug.dylib",
    "name" : "Runner.debug.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4378607616,
    "CFBundleShortVersionString" : "2.4.0",
    "CFBundleIdentifier" : "org.cocoapods.FBLPromises",
    "size" : 81920,
    "uuid" : "816d9f36-de82-38b4-b148-f613efc7a3d4",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/FBLPromises.framework\/FBLPromises",
    "name" : "FBLPromises",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4378820608,
    "CFBundleShortVersionString" : "11.15.0",
    "CFBundleIdentifier" : "org.cocoapods.FirebaseCore",
    "size" : 81920,
    "uuid" : "e7e3724f-2488-3765-bf88-6200ae787e5c",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/FirebaseCore.framework\/FirebaseCore",
    "name" : "FirebaseCore",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4379541504,
    "CFBundleShortVersionString" : "11.15.0",
    "CFBundleIdentifier" : "org.cocoapods.FirebaseCoreInternal",
    "size" : 163840,
    "uuid" : "a4f2fa2f-c540-393b-a11c-c3b53dc27f62",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/FirebaseCoreInternal.framework\/FirebaseCoreInternal",
    "name" : "FirebaseCoreInternal",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4377214976,
    "CFBundleShortVersionString" : "11.15.0",
    "CFBundleIdentifier" : "org.cocoapods.FirebaseInstallations",
    "size" : 114688,
    "uuid" : "05c04aa7-e5bc-32f3-8ea8-d32f7b76ed3e",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/FirebaseInstallations.framework\/FirebaseInstallations",
    "name" : "FirebaseInstallations",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4382113792,
    "CFBundleShortVersionString" : "11.15.0",
    "CFBundleIdentifier" : "org.cocoapods.FirebaseMessaging",
    "size" : 294912,
    "uuid" : "086af4b4-718c-3710-aacc-600a5c29e2f7",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/FirebaseMessaging.framework\/FirebaseMessaging",
    "name" : "FirebaseMessaging",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4380033024,
    "CFBundleShortVersionString" : "10.1.0",
    "CFBundleIdentifier" : "org.cocoapods.GoogleDataTransport",
    "size" : 212992,
    "uuid" : "cdb43475-0dc1-3609-981a-ee87e1b1c04b",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/GoogleDataTransport.framework\/GoogleDataTransport",
    "name" : "GoogleDataTransport",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4380475392,
    "CFBundleShortVersionString" : "8.1.0",
    "CFBundleIdentifier" : "org.cocoapods.GoogleUtilities",
    "size" : 147456,
    "uuid" : "2075202e-6e64-3d62-a63b-0a5ecd75a788",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/GoogleUtilities.framework\/GoogleUtilities",
    "name" : "GoogleUtilities",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4379148288,
    "CFBundleShortVersionString" : "3.30910.0",
    "CFBundleIdentifier" : "org.cocoapods.nanopb",
    "size" : 32768,
    "uuid" : "3a5a611f-5724-3a28-b7b9-df720d86947a",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/nanopb.framework\/nanopb",
    "name" : "nanopb",
    "CFBundleVersion" : "1"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4431167488,
    "CFBundleShortVersionString" : "1.0",
    "CFBundleIdentifier" : "io.flutter.flutter",
    "size" : 35110912,
    "uuid" : "4c4c4486-5555-3144-a1c4-573fe7e1e08b",
    "path" : "\/Users\/USER\/Library\/Developer\/CoreSimulator\/Devices\/2252DDC0-C915-4B0C-8C71-B97C2BC60A03\/data\/Containers\/Bundle\/Application\/36717FEF-7EF1-446C-B139-C4667172DBCD\/Runner.app\/Frameworks\/Flutter.framework\/Flutter",
    "name" : "Flutter",
    "CFBundleVersion" : "1.0"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4379246592,
    "size" : 32768,
    "uuid" : "93afc0a9-eec9-3f50-9339-09c7757aa50a",
    "path" : "\/usr\/lib\/system\/libsystem_platform.dylib",
    "name" : "libsystem_platform.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4384047104,
    "size" : 245760,
    "uuid" : "4068b2ee-a54f-397e-882d-c5e3a40b789a",
    "path" : "\/usr\/lib\/system\/libsystem_kernel.dylib",
    "name" : "libsystem_kernel.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4383211520,
    "size" : 65536,
    "uuid" : "e9238785-e581-3e65-bedb-179c698d3554",
    "path" : "\/usr\/lib\/system\/libsystem_pthread.dylib",
    "name" : "libsystem_pthread.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 4383883264,
    "size" : 49152,
    "uuid" : "67028e6c-ae93-39e7-b3c8-6f6edf1cd0a5",
    "path" : "\/Volumes\/VOLUME\/*\/libobjc-trampolines.dylib",
    "name" : "libobjc-trampolines.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6443732992,
    "size" : 512744,
    "uuid" : "11b4e598-e39a-34a8-9420-9a309c31374d",
    "path" : "\/Volumes\/VOLUME\/*\/libsystem_c.dylib",
    "name" : "libsystem_c.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6445473792,
    "size" : 99696,
    "uuid" : "1bce4456-2666-3573-a2b6-1a4e9fb5376a",
    "path" : "\/Volumes\/VOLUME\/*\/libc++abi.dylib",
    "name" : "libc++abi.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6442909696,
    "size" : 250068,
    "uuid" : "0fe5d25f-a499-3820-a943-bb603064bf8c",
    "path" : "\/Volumes\/VOLUME\/*\/libobjc.A.dylib",
    "name" : "libobjc.A.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6446329856,
    "CFBundleShortVersionString" : "6.9",
    "CFBundleIdentifier" : "com.apple.CoreFoundation",
    "size" : 4319072,
    "uuid" : "189f2366-e917-3261-ba91-1c8d562f613f",
    "path" : "\/Volumes\/VOLUME\/*\/CoreFoundation.framework\/CoreFoundation",
    "name" : "CoreFoundation",
    "CFBundleVersion" : "4034.1.101"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6527746048,
    "CFBundleShortVersionString" : "1.0",
    "CFBundleIdentifier" : "com.apple.UIKitCore",
    "size" : 34742624,
    "uuid" : "ac67e1bc-cacf-3e1b-b45b-fe58b192b4ac",
    "path" : "\/Volumes\/VOLUME\/*\/UIKitCore.framework\/UIKitCore",
    "name" : "UIKitCore",
    "CFBundleVersion" : "9079.2.105"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6581407744,
    "CFBundleShortVersionString" : "996",
    "CFBundleIdentifier" : "com.apple.FrontBoardServices",
    "size" : 837952,
    "uuid" : "d5e3a78f-ea5a-34aa-82b4-53d213d9b4d3",
    "path" : "\/Volumes\/VOLUME\/*\/FrontBoardServices.framework\/FrontBoardServices",
    "name" : "FrontBoardServices",
    "CFBundleVersion" : "996"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6444249088,
    "size" : 283072,
    "uuid" : "59a93b97-f29b-3393-8914-4559ba560b73",
    "path" : "\/Volumes\/VOLUME\/*\/libdispatch.dylib",
    "name" : "libdispatch.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6575497216,
    "CFBundleShortVersionString" : "1.0",
    "CFBundleIdentifier" : "com.apple.BoardServices",
    "size" : 516288,
    "uuid" : "2c074346-da2b-35ae-81f1-20aeb1ddd4f9",
    "path" : "\/Volumes\/VOLUME\/*\/BoardServices.framework\/BoardServices",
    "name" : "BoardServices",
    "CFBundleVersion" : "732"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6753677312,
    "CFBundleShortVersionString" : "1.0",
    "CFBundleIdentifier" : "com.apple.GraphicsServices",
    "size" : 32192,
    "uuid" : "96b4e580-68f1-3d45-99c9-d40edf82691e",
    "path" : "\/Volumes\/VOLUME\/*\/GraphicsServices.framework\/GraphicsServices",
    "name" : "GraphicsServices",
    "CFBundleVersion" : "1.0"
  },
  {
    "size" : 0,
    "source" : "A",
    "base" : 0,
    "uuid" : "00000000-0000-0000-0000-000000000000"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6443343872,
    "size" : 122592,
    "uuid" : "81b58298-cefa-30ff-b54e-04d292715805",
    "path" : "\/Volumes\/VOLUME\/*\/libsystem_trace.dylib",
    "name" : "libsystem_trace.dylib"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6451171328,
    "CFBundleShortVersionString" : "6.9",
    "CFBundleIdentifier" : "com.apple.Foundation",
    "size" : 14084064,
    "uuid" : "8cd46c12-9968-3222-864d-c654dab3d116",
    "path" : "\/Volumes\/VOLUME\/*\/Foundation.framework\/Foundation",
    "name" : "Foundation",
    "CFBundleVersion" : "4034.1.101"
  },
  {
    "source" : "P",
    "arch" : "arm64",
    "base" : 6443466752,
    "size" : 252192,
    "uuid" : "fff02806-1f2a-3c70-9455-959fffe4edb7",
    "path" : "\/Volumes\/VOLUME\/*\/libxpc.dylib",
    "name" : "libxpc.dylib"
  }
],
  "sharedCache" : {
  "base" : 6442450944,
  "size" : 4268605440,
  "uuid" : "a397ca0d-86b3-3756-917e-6490980f584a"
},
  "vmSummary" : "ReadOnly portion of Libraries: Total=1.3G resident=0K(0%) swapped_out_or_unallocated=1.3G(100%)\nWritable regions: Total=680.5M written=1927K(0%) resident=1927K(0%) swapped_out=0K(0%) unallocated=678.7M(100%)\n\n                                VIRTUAL   REGION \nREGION TYPE                        SIZE    COUNT (non-coalesced) \n===========                     =======  ======= \nActivity Tracing                   256K        1 \nColorSync                           64K        4 \nFoundation                          16K        1 \nKernel Alloc Once                   32K        1 \nMALLOC                           616.6M       42 \nMALLOC guard page                  128K        8 \nSTACK GUARD                       56.3M       20 \nStack                             25.6M       20 \nVM_ALLOCATE                       37.6M       48 \n__DATA                            18.5M      476 \n__DATA_CONST                      66.7M      499 \n__DATA_DIRTY                        91K       13 \n__FONT_DATA                        2352        1 \n__LINKEDIT                       713.9M       17 \n__OBJC_RO                         63.2M        1 \n__OBJC_RW                         2847K        1 \n__TEXT                           641.9M      512 \n__TPRO_CONST                       148K        2 \ndyld private memory                2.2G       12 \nmapped file                       34.7M       13 \npage table in kernel              1927K        1 \nshared memory                       16K        1 \n===========                     =======  ======= \nTOTAL                              4.4G     1694 \n",
  "legacyInfo" : {
  "threadTriggered" : {
    "queue" : "com.apple.main-thread"
  }
},
  "logWritingSignature" : "cae9c6fb3c5972a601b1e252cbf3d35c5977f37d",
  "trialInfo" : {
  "rollouts" : [
    {
      "rolloutId" : "67648e5334a82511f4acf879",
      "factorPackIds" : {

      },
      "deploymentId" : 240000008
    },
    {
      "rolloutId" : "6297d96be2c9387df974efa4",
      "factorPackIds" : {

      },
      "deploymentId" : 240000032
    }
  ],
  "experiments" : [

  ]
}
}

Model: Mac14,9, BootROM 11881.121.1, proc 12:8:4 processors, 16 GB, SMC 
Graphics: Apple M2 Pro, Apple M2 Pro, Built-In
Display: Color LCD, 3024 x 1964 Retina, Main, MirrorOff, Online
Display: HP 27xw, 1920 x 1080 (1080p FHD - Full High Definition), MirrorOff, Online
Memory Module: LPDDR5, Hynix
AirPort: spairport_wireless_card_type_wifi (0x14E4, 0x4388), wl0: Mar 22 2025 02:16:34 version 23.40.30.0.41.51.180 FWID 01-5f726d72
IO80211_driverkit-1475.39 "IO80211_driverkit-1475.39" Apr 18 2025 20:10:40
AirPort: 
Bluetooth: Version (null), 0 services, 0 devices, 0 incoming serial ports
Network Service: Wi-Fi, AirPort, en0
USB Device: USB31Bus
USB Device: USB31Bus
USB Device: USB3.1 Hub
USB Device: USB2.1 Hub
USB Device: iPhone
USB Device: USB2.0 Hub
USB Device: USB Receiver
USB Device: USB Type-C Digital AV Adapter
USB Device: USB Storage
USB Device: USB31Bus
Thunderbolt Bus: MacBook Pro, Apple Inc.
Thunderbolt Bus: MacBook Pro, Apple Inc.
Thunderbolt Bus: MacBook Pro, Apple Inc.

