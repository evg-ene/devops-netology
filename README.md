# Домашнее задание к занятию «2.4. Инструменты Git»
## Ответы на вопросы:
1. aefead2207ef7e2aa5dc81a34aedf0cad4c32545
   1. git show aefea
2. tag: v0.12.23
   1. git show 85024d3 --tags
3. Два (56cd7859e и 9ea88f22f)
   1. git log --pretty=%p -n 1 b8d720
4. Коммиты между тегами v0.12.23 и v0.12.24
   1. git log v0.12.23..v0.12.24 --oneline
      - 33ff1c03b (tag: v0.12.24) v0.12.24
      - b14b74c49 [Website] vmc provider links
      - 3f235065b Update CHANGELOG.md
      - 6ae64e247 registry: Fix panic when server is unreachable
      - 5c619ca1b website: Remove links to the getting started guide's old location
      - 06275647e Update CHANGELOG.md
      - d5f9411f5 command: Fix bug when using terraform login on Windows
      - 4b6d06cc5 Update CHANGELOG.md
      - dd01a3507 Update CHANGELOG.md
      - 225466bc3 Cleanup after v0.12.23 release
      - 85024d310 (tag: v0.12.23) v0.12.23
5. 8c928e835 main: Consult local directories as potential mirrors of providers
   1. git log -S'func providerSource' --oneline
6. Коммиты в которых изменили функцию globalPluginDirs
   1. git log --pretty=%p - получил файл, где находиться данная функция
   2. git log -L :globalPluginDirs:plugins.go --oneline
      - 78b122055 Remove config.go and update things using its aliases
      - 52dbf9483 keep .terraform.d/plugins for discovery
      - 41ab0aef7 Add missing OS_ARCH dir to global plugin paths
      - 66ebff90c move some more plugin search path logic to command
      - 8364383c3 Push plugin discovery down into command package
7. Author: Martin Atkins <mart@degeneration.co.uk>
   1. git log -S'synchronizedWriters' --oneline --pretty=%an
