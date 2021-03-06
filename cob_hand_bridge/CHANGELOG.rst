^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package cob_hand_bridge
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.6.1 (2016-10-10)
------------------
* fix install tags
* move launch files to bringup
* start init server after status topic is connected
* speed-up line parsing
* fixed offset calculation bug
* stop timer on preemption
* improved deadline timer
* fixed typo in JointValues.msg
* resend while moving
* set nominal current as default
* renamed g_motors_stopped to to g_motion_stopped
* resend only if control was stopped
* set default velocity (unused, but must be in valid range)
* move command string format was wrong, updated to signed
* pass currents to SDHx
* read currents from trajectory
* parse default currents
* non-positive resend_timer disables it
* stop resending on error
* use deadline timer instead of resend timer
* properly handle goal if already at target
* added missing dependency
* Fix for `#6 <https://github.com/ipa320/cob_hand/issues/6>`_, added dependency to self
* deep-copy port string
* require movement to start
* migrated to goalCB
* increased stopped velocity
* support trajectories with missing header stamp
* proper conversions
* do not test for tolerances size (outdated code)
* catch not connected error in init
* first status detected was buggy
* finger ready  logic was inverted
* added trajectory interface
* wait for init_finger service
* enable recover on non-zero RC
* Use global namespaces to make remap work
* Do not check required interfase per default
  rosserial checks FQN, does not work with component namespaces
* report error on non-zero SDHx return code
* added diagnostics
* c&p bug
* device port was missing the leading slash
* resize position vector before filling it
* advertise recover service
* updated mismatched MD5 sums
* added first version of node
* implemented recover service
* actually read velocity and current from SDHx
* switched to signed current entry
* improved line parsing
* Keep existing PWM setting if value is zero
* Create README.md
* PWM just works for first bank
* added launch file
* refactored for PWM feature
* added support for bank1
* removed sdhx.cpp from CMake config
* SDHx implementation
* first test app with GPIO
* Contributors: Florian Weisshardt, Mathias Lüdtke, ipa-cob4-5, ipa-nhg
