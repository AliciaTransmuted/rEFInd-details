![Screenshot](https://i.imgur.com/8s2cobL.png)

# rEFInd-details
A colourful theme for the rEFInd UEFI boot manager

[rEFInd](http://www.rodsbooks.com/refind/) is a boot manager for UEFI systems and scans for kernels & EFI at boot.

### Usage

 1. Locate your refind EFI directory. This is commonly `/boot/EFI/refind`
    though it will depend on where you mount your ESP and where rEFInd is
    installed.

 2. Create a folder called `themes` inside it, if it doesn't already exist

 3. Clone this repository into the `themes` directory as `themes/rEFInd-details`.

 4. To enable the theme add `include themes/rEFInd-details/theme.conf` at the end of
    `refind.conf`.
    
Entries should be autodetected and shown with the proper icons.

Manual entry can be done via `menuentry` option.

Example:

```
menuentry "Windows" {
	icon /EFI/refind/themes/rEFInd-details/icons/os_windows.png
	loader /EFI/Microsoft/Boot/bootmgfw.efi
}
```

Other examples are in the `refind.conf` file.

-------------------------------
rEFInd-details notes
-------------------------------

September 10, 2018
Initial release of rEFInd-details to DeviantArt.
Many new product icons were added in this release.
All icons were recreated and/or redesigned with the goal of making them consistent, attractive and intuitive.
The background image, called "Details", is one of my photographs.

December 30, 2018: rEFInd-details theme uploaded to github.
