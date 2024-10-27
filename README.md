# DNPERF
## List of changes
- Port some functions of d3dx9math to DXMATH (compiled with AVX)
- Ice stacks attaches only once. (Damage is still the same, but I might find an alternative without affect the visuals)
- Removed a lot of Critical Sections.
- Increased FPS on 8man (raid) or 8v8 PVP repsawn
- Removed equipment score for less stuttery when browsing/comparing equipments

## List of did not fix (might be a TODO)
- Micro-stutters/stutters (most likely heap related or reading files that blocks the thread)
- Bad frametime (idk)

## How to use it
```
└── Dragon Nest Folder
    ├── netapi32.dll
    └── dragonnest_x64.exe
```
## Client
Official clients only. 

## Issue
If you found an issue while using this, please create an issue on [Issues Section](https://github.com/dnblank123/dnperf-public/issues), and make sure to test it thoroughly, without and with the mod. If the issue is hard to notice, attach a video, otherwise, attach a picture.