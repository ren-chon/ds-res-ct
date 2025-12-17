# Resolution Patch
## Quick Start

1. **Download and install** [Cheat Engine](https://www.cheatengine.org/)
2. **Launch the game** (ds.exe)
3. **Open Cheat Engine** and click the computer icon (top-left)
4. **Select "ds.exe"** from the process list
5. **Load the script**: Click `File > Load` and select the `.CT` file you just downloaded
6. **Activate the patch**: Check the box next to the resolution name
7. **Test the resolution**: Go to game settings, select any resolution and Apply
8. **Done!** Your game should now run at your desired resolution

---

## Custom Resolution

Edit the script before activating:

1. **Right-click** the any resolution entry → Select `Change script`
2. **Find these two lines**:
   ```
   mov eax,<WIDTH in hex>
   mov ecx,<HEIGHT in hex>
   ```
3. **Replace the hex values**:
   - `F00` = Width (3840 in hex)
   - `654` = Height (1620 in hex)
4. **Convert your desired resolution** to hexadecimal:
   - Use [RapidTables Converter](https://www.rapidtables.com/convert/number/decimal-to-hex.html)
   - Copy the value inside 'Hex number (3 digits)'
5. **Update the values** and click `OK`
6. **Activate** the checkbox to apply

**Example for 1920x1080**:
```
mov eax,780
mov ecx,438
```

---

## Troubleshooting

- **Game crashes?** Make sure ds.exe is running before attaching Cheat Engine
- **Resolution not changing?** Verify the script is checked/enabled
- **Wrong resolution?** Double-check your hex conversion
- **Still not working?** Try restarting the game and reattaching Cheat Engine

---

## Important Notes

- This modifies game memory temporarily - changes reset when you close the game
- Some resolutions may cause UI issues or graphical glitches
