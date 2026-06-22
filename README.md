# PandaKB Sofle

![Sofle keymap](keymap-drawer/Sofle.svg)

Диаграмма раскладки генерируется автоматически из [`config/Sofle.keymap`](config/Sofle.keymap) при push через [keymap-drawer](https://github.com/caksoylar/keymap-drawer) (workflow [Draw ZMK keymaps](.github/workflows/draw-keymaps.yml)).

Описание решений по раскладке: [`config/KEYMAP.md`](config/KEYMAP.md).

После первого push в ветку `keymap-drawer` GitHub Actions создаст `keymap-drawer/Sofle.svg` и закоммитит его.

## Энкодеры

Энкодеры не припаяны, но shield включает их в devicetree — для сборки нужны `CONFIG_EC11=y`, `CONFIG_EC11_TRIGGER_GLOBAL_THREAD=y` и `sensor-bindings` на каждом слое в [`config/Sofle.keymap`](config/Sofle.keymap).
