## 2.0.0

 - fix!: `push` & `unshift` now accept `undefined` values to match behaviour of `Array` (fixes #25) (#35)
   - This is only a **BREAKING** change if you are currently expecting `push(undefined)` and `unshift(undefined)` to do
     nothing - the new behaviour now correctly adds undefined values to the queue.
   - **Note**: behaviour of `push()` & `unshift()` (no arguments) remains unchanged (nothing gets added to the queue).
   - **Note**: If you need to differentiate between `undefined` values in the queue and the return value of `pop()` then
     check the queue `.length` before popping.
 - fix: incorrect methods in types definition file

## 1.5.1

 - perf: minor performance tweak when growing queue size (#29)

## 1.5.0

 - feat: adds capacity option for circular buffers (#27)

