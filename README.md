# FFmpeg-in-Xcode

- A project for debugging FFmpeg and SDL in Xcode.

## Condition

- FFmpeg : 4.1
- configuration  : --disable-asm

## Schemes

- Run ffmpeg, ffplay, or ffprobe.

![schemes](https://github.com/libobjc/FFmpeg-in-Xcode/blob/master/snapshot/schemes.png?raw=true)

## Arguments

- Add launch arguments at ‘Edit Scheme’ panel.

![arguments](https://github.com/libobjc/FFmpeg-in-Xcode/blob/master/snapshot/arguments.png?raw=true)

## How to use?

1. Clone this repo.
1. Direct run ffmpeg, ffplay, or ffprobe.

## How to customize?

##### The project provides a tool to simply change the FFmpeg version and configuration.

1. Download FFmpeg source, configure and make.
1. Remove FFmpeg source files from project.
1. Open 'build.m', Replace to your own FFmpeg and project paths.
1. Select scheme to build-1, and run it.
1. Add the files under $(ProjectRoot)/FFmpeg to the project(target is FFmpeg, fftools except).
1. Configure fftools to correct target. Refer to existing project 'Target Membership'.
1. Select scheme to build-2, and run it.
1. Done.

#### You can view snapshot of the key node in the snapshot directory.
Fix include for apple M1
<img width="456" alt="Screenshot 2023-11-09 at 16 47 20" src="https://github.com/lazyduck037/FFmpeg-in-Xcode/assets/32600174/8ac575c3-0386-45c8-bef0-37d378f07300">


