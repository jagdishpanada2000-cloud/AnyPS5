# libSceNpCommon

## add Functional

- [sceNpUtilGetNthChar guest source](../../../core/libs/prx/libSceNpCommon/Strings.cpp) (libSceNpCommon) - reads the NUL-terminated guest text through GuestCopyIn_nid_no_patch before counting characters, bounds multibyte validation to the copied text, and returns the corresponding offset in the original guest string; returning 0x80550601 for an unreadable source is a host-safety fallback with console behaviour unmeasured.
