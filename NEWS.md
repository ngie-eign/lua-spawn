## 0.2 - 2026-XX-YY

### Feature Enhancements

- Add support for Lua 5.4 and 5.5.
- Allow passing `nil` as posix_spawn file actions and attributes to match the
  `posix_spawn*` APIs with `NULL`.

### Bugfixes
- Make code ANSI-C clean.
- Use raw operations instead of dynamic strings to fix `lua_geti` use in posix module.
- Fix build on OSes where `O_*SYNC` flags aren't implemented, e.g., FreeBSD.
- Fix feature check for `_POSIX_PRIORITY_SCHEDULING` to unbreak the build on macOS with llvm.

### Documentation
- Document `luarocks` install process.

## 0.1 - 2018-08-10

- Initial release
