# vcpkg-craftinfo

Craftinfo for mulle-sde to build [vcpkg](//github.com/microsoft/vcpkg). This
calls the installer and copies vcpkg into `dependency`.

The vcpkg folder will be in the project root.


``` bash
mulle-sde dependency add --github microsoft vcpkg
mulle-sde dependency mark vcpkg singlephase
mulle-sde environment --global set --concat MULLE_CRAFT_USE_SCRIPTS vcpkg-build
```
