DOWNLOAD PLUGIN BINARIES FOR WINDOWS AND LINUX HEEE.
https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/releases

# Gimp Plugin to make equal pie dividers.

Render Equal Pie Slices with this Gimp plugin. Though in default it is a four cornered structure. Rotating and adding dividers makes it looks like pie.

Example of the plugin in action below

**Plugin, rendering the equal dividers**
![image](https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/assets/78667207/24759b95-30f3-4d84-b023-f836448ea224)

**Manual labor aspect of plugin**
![image](https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/assets/78667207/ab3ea980-d7e8-4532-91e8-ce4e87f8c0ea)


**End result of manual labor**
![image](https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/assets/78667207/dd4b5d85-8eba-4246-adee-2246b14e6f9c)

Location to put binaries

**Windows**

 C:\Users\(USERNAME)\AppData\Local\gegl-0.4\plug-ins
 
 **Linux** 

 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
**Linux (Flatpak includes Chromebook)**

 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

After installing, restart Gimp and go to GEGL Operations. Look for the name Pie Divider.
If you have Gimp 2.99.16 this plugin will be found in filters>render>fun.

## Compiling and Installing

### Linux

To compile and install you will need the GEGL header files (`libgegl-dev` on
Debian based distributions or `gegl` on Arch Linux) and meson (`meson` on
most distributions).

```bash
meson setup --buildtype=release build
ninja -C build

```

If you have an older version of gegl you may need to copy to `~/.local/share/gegl-0.3/plug-ins`
instead (on Ubuntu 18.04 for example).

BEAVER RECOMMENDS YOU USE A MODERN VERSION OF GEGL. NO GUARANTEE DATED VERSIONS OF GIMP WILL WORK WITH THIS PLUGIN 

### Windows

The easiest way to compile this project on Windows is by using msys2.  Download
and install it from here: https://www.msys2.org/

Open a msys2 terminal with `C:\msys64\mingw64.exe`.  Run the following to
install required build dependencies:

```bash
pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl
```

Then build the same way you would on Linux:

```bash
meson setup --buildtype=release build
ninja -C build
```

## More Previews of the plugins options

![image](https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/assets/78667207/30bd61f8-5ff7-45b8-9b7d-c7213ab6fbc2)

![image](https://github.com/LinuxBeaver/Gimp_Plugin_Equal_Pie_Divider/assets/78667207/932da5d1-bd8c-4a33-847d-a911eedf970f)



