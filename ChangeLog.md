## v0.3.2

### Bug fixes

- Fix undefined behavior due to incorrect usage of `isprint` function.

### Internal

- Fix compilation for compilers other than gcc, clang, msvc.
- Add build with tcc to CI.
- Rewrote `mk_wcwidth` function.

## v0.3.1

### Bug fixes

- Fix incorrect behaviour when setting properties with `FT_CUR_...` macroses.

## v0.3.0

### API

- Changes in C++ API (introduced classes `char_table` and `utf8-table` instead of `table`).
- Add function `ft_set_u8strwid_func` to set custom function to compute width of utf8 strings.

### Internal

- Refactoring of examples.

## v0.2.2

### Bug fixes

- Fix incorrect behaviour in case of wide east asian symbols.

## v0.2.1

### Bug fixes

- Fix incorrect `ft_u8nwrite` implementation.

## v0.2.0

### API

- Added support for UTF-8 strings (`ft_u8write`, `ft_u8printf` ...).
- Added getters for current cell (`cur_col`, `cur_row`, `cur_cell`) to C++ API.
- Enabled wide character and UTF-8 support by default.

### Internal

- Code refactoring.

## v0.1.6

### Internal

- Removed blank lines from `PLAIN_STYLE` and `SIMPLE_STYLE`.

### Bug fixes

- Changed specific style reset tags to universal reset style tag.
- Fix incorrect border style for the last line in the table.

### Tests

- Added more tests for border styles.

## v0.1.5

### Tests

- Add tests for 'mk_wcswidth' function.

## v0.1.4

### Internal

- Removed redundant build options from cmake files.
- Added build for arm platform with drone.ci.

## v0.1.3

### Internal

- Fixed error with incorrect types when determine class of 'wchar_t' symbol for platforms with unsigned 'wchar_t'.

## v0.1.2

### Internal

- Removed '-Werror' flag from the build process.

## v0.1.1

### Internal

- Add library version and soversion to the built library.

## v0.1.0

Initial release
