### Description
Add swipe gestures to trigger functions, similar to [libinput-gestures](https://github.com/bulletmark/libinput-gestures/tree/master). It supports the following gestures: `SWIPE_UP`, `SWIPE_DOWN`, `SWIPE_LEFT` and `SWIPE_RIGHT`

> NOTE: It requires that you have previously applied [pointer-gestures-unstable-v1](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/pointer-gestures-unstable-v1)

```c
static const Gesture gestures[] = {
  /* modifier gesture       fingers_count   function    argument */
  { MODKEY,   SWIPE_LEFT,   4,              shiftview,  { .i = 1 } },
  { 0,        SWIPE_RIGHT,  4,              shiftview,  { .i = -1 } },
};
```

**NOTE:** the example above requires the following patch [shiftview](https://codeberg.org/dwl/dwl-patches/wiki/shiftview)

### Download
- [git branch](https://codeberg.org/wochap/dwl/src/branch/v0.5/gestures)
- [2024-07-09](https://codeberg.org/dwl/dwl-patches/raw/commit/13d96b51b54500dd24544cf3a73c61b7a1414bc6/patches/gestures/gestures.patch)
- [2024-04-11](https://codeberg.org/dwl/dwl-patches/raw/commit/be3735bc6a5c64ff76c200a8679453bd179be456/gestures/gestures.patch)
- [v0.5](https://codeberg.org/dwl/dwl-patches/raw/commit/655fd2916c1bcaa022ce6dcdfb370051cf64df66/gestures/gestures.patch)

### Authors
- [wochap](https://codeberg.org/wochap)
