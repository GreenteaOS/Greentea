## Monolithic rolling-release updates of the system

Basic idea is to download a single system image via p2p-sharing (and do integrity checks, of course) and place it packed to the system partition as-is. Images a kept unchanged, and unpacked on-demand into RAM. They should contain kernel, common drivers and built-in apps.

This will gave nearly instantaneous updates with improved system resilience.
