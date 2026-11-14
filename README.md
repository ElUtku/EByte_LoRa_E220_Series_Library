# EByte LoRa E220 Series Library (fork)

This is a fork of [xreef/EByte_LoRa_E220_Series_Library](https://github.com/xreef/EByte_LoRa_E220_Series_Library) by Renzo Mischianti ([www.mischianti.org](https://www.mischianti.org)), distributed under the original MIT license (see [`LICENSE.md`](LICENSE.md)).

For full documentation, tutorials, wiring and examples, see the original repository and <https://www.mischianti.org/category/my-libraries/ebyte-lora-e22-devices/>.

## Change in this fork

`DEBUG_PRINTER` can be overridden from outside the library, and a custom header can be included with `DEBUG_PRINTER_HEADER`. The default behaviour (`Serial`) is unchanged.

```ini
; platformio.ini
build_flags =
    -DLoRa_E220_DEBUG
    -DDEBUG_PRINTER_HEADER=\"my_log.h\"
    -DDEBUG_PRINTER=MyLog

lib_deps =
    https://github.com/ElUtku/EByte_LoRa_E220_Series_Library.git#v1.0.8-debugprinter
```
