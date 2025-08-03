# DNPERF
## Official clients and DX11 only.
> - Tested on SEA. 
> - No private server support.

## Disclaimer
**Use at your own risk, especially getting banned or losing your raids.** I haven't fully tested this on raids, only tested in towns and PVP 8v8.

## List of changes
- Port some functions of d3dx9math to DXMATH (compiled with AVX)
- Ice stacks attach only once.
> - (Damage is still the same, ~~but I might find an alternative without affecting the visuals. Currently found a workaround and implementing it as soon as possible)~~. Will be sticking with "attach only once". It still frame drops with the other workaround.
- Removed a lot of Critical Sections.
- Increased FPS on 8man (raid) or 8v8 PVP repsawn
- Removed equipment score for less stuttery when browsing/comparing equipments
- Port zlib to zlib-ng (with runtime check to use SSE/AVX/AVX2/AVX512 etc)
- Faster C libraries with SIMD (runtime check to use SSE/AVX)
- Fixed memory leaks (total of 2)
- Removed FXAA
- Removed restore audio
- Fix misaligned particles (Works on DX9).
- vcruntime140 for AVX2 memcpy/memset
- Much faster loading on start with a total time of 6 seconds. (on my PC)
- High resolution timer for sleep
## Upcoming releases
- 

## List of did not fix (might be a TODO)
- Micro-stutters/stutters (most likely heap related or reading files that blocks the thread)
- Better frametime
- Find and fix memory leak
## How to use it
```
└── Dragon Nest Folder
    ├── netapi32.dll
    └── dragonnest_x64.exe
```

## Where source code?
Yeah no. Guess it why.

## Issue
If you found an issue while using this, please create an issue on [Issues Section](https://github.com/grazaerd/dnperf-public/issues), and make sure to test it thoroughly, without and with the mod. If the issue is hard to notice, attach a video, otherwise, attach a picture.