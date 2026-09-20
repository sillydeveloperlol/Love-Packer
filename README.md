# LÖVE Packer

A simple tool for packaging your [LÖVE](https://love2d.org/) game project into a single `.love` file.

No command line required just select your project, choose where you want the `.love` file, and let LÖVE Packer handle the rest.

---

## 📦 Tutorial

### 1. Download LÖVE Packer

Download the latest release of **LÖVE Packer** from the Releases page.

### 2. Run the application

Open the `.exe` file you downloaded.

> **Windows Security Warning**
>
> Windows may display a message saying that it protected your PC.
>
> If this happens, click **More info**, then click **Run anyway**.
>
> This can happen because the application is not currently code-signed.

### 3. Select your project

When LÖVE Packer opens:

1. Click **Choose Project**.
2. Select the **root folder** of your LÖVE project.

Your project should look something like:

```text
MyGame/
├── conf.lua
├── main.lua
├── assets/
│   ├── player.png
│   └── music.ogg
└── ...
```

**Important:** Select the folder containing `main.lua` and `conf.lua`, not one of the folders inside your project.

### 4. Choose an output location

Click **Choose Location** and select where you want your `.love` file to be created.

> ⚠️ **Known issue**
>
> As of the latest release, the automatic output-folder selection does not work correctly and may cause an error.
>
> **Please manually select an output folder.**

### 5. Pack your game

Click **Pack Game** and wait for the status to say:

**● Packed successfully**

Your `.love` file will be created in the output folder you selected.

### 6. Find your `.love` file

The output file will use your project's folder name.

For example:

```text
MyGame/
    ↓
MyGame.love
```

> **Desktop note**
>
> If you selected your Desktop as the output location, the file may not immediately appear on your desktop.
>
> Don't worry the file should still be inside your Desktop folder. Open **File Explorer** and navigate to your Desktop to find it.

---

## 🛠️ What is LÖVE Packer?

LÖVE Packer takes the files in your LÖVE project and packages them into the `.love` archive format required by the LÖVE game engine.

Instead of manually creating a ZIP archive and renaming it to `.love`, LÖVE Packer does it for you.

### Before

```text
MyGame/
├── conf.lua
├── main.lua
└── assets/
    └── player.png
```

### After

```text
MyGame.love
```

That's it. Your entire project is packaged into one file.

---

## ⚠️ Known Issues

* Automatic output-folder selection may not work in the latest release. Manually select an output folder instead.
* Windows SmartScreen may display a warning because the application is not currently code-signed.
* Files may take a moment to appear when using the Desktop as the output location.

---

## Planned Changes

* Changing default output location from `Desktop` to the folder you chose for the project

---

## 📋 Requirements

For the packaged `.exe`, **no Python installation is required**.

Just download the latest release and run the executable.

---

## ❤️ Made for LÖVE

Built to make packaging LÖVE projects a little less annoying.

Have fun making games!
