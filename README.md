# Ghidra Wii U Datatypes

This repo contains datatypes based on [wut 1.3.2-b98f8fc](https://github.com/devkitPro/wut/commit/b98f8fc824409a4ae8fa79e32b1a6c0da21501b2).

Parsing the wut header is not perfect. Make sure to keep the following in mind when using this wut datatype.
- It may contain duplicated structs due to forwards declaration.
- Any structs that uses `WUT_PACKED` may have the wrong size (as the packed attributed it not parsed).
- Some structs may have missing attributes. This happened during clean-up of duplicated structs.