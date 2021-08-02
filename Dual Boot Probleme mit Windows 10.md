# Dual Boot Probleme mit Windows 10

*Im Code ist Ubuntu nur ein Platzhalter für die jeweilige Distribution*

## Bootloader hinzufügen

Wenn das BIOS/UEFI den Grub-Bootloader nicht findet, kann dieser wie folgt angegeben werden:

*Eingabeaufforderung als Administrator starten*

```powershell
bcdedit /set {bootmgr} path \EFI\ubuntu\grubx64.efi
```

## Bootloader entfernen

*Eingabeaufforderung als Administrator starten*

```powershell
diskpart
list disk
sel disk (passende Nummer für Fesplatte)
list vol
sel vol (passende Nummer für System)
assign letter=X: (freien Buchstaben verwenden)
exit
X:
dir (EFI sollte hier zu finden sein)
cd EFI
dir (passender Ordner sollte hier zu finden sein)
rmdir /S ubuntu
```

## Quellen

- [Dual boot not working in windows 10](https://askubuntu.com/questions/893559/dual-boot-not-working-in-windows-10#893568)

- [Uninstall GRUB and use Windows bootloader](https://askubuntu.com/questions/429610/uninstall-grub-and-use-windows-bootloader#869888)