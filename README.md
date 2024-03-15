# Meta-Port

### STATUS: WORKING
- It works as intended, there will be, limited or no, further development.

## DESCRIPTION
This is a batch that neatly runs MetaTrader in Portable mode, as such it uses its own directory to store all the files. There are 2 reasons you may want to do this, I use it for both these reasons...
1. To not run out of activations on Expert Advisors, for example when you reinstall the OS.
2. Run multiple accounts on the same machine, for example, one for forex and one for commodities.

### FEATURES
- **Clear Interface**: Text confirmations with short wait commands, explaining what is going on.
- **Self-Termination**: The batch closes itself after running MetaTrader.

### PREVIEW
- No frills here yet...
```

Script Initialized...


Launching MetaTrader 5 in Portable Mode..
..MetaTrader 5 Launched.


...Script Complete.











```


## REQUIREMENTS
- Windows with scripting host enabled.
- Installation of MetaTrader 5.

### USAGE
1. Copy your MetaTrader 5 program directory to a safe location, such as for example `DRIVE:\PARENT FOLDER\Meta-Port`, somewhere that dont have permission issues, ie not `C:\Program Files\SOME FOLDER`.
2. Put, `Port-Trade.Bat` and `Port-Edit.Bat` (if you use it), in same dir as "Terminal64.exe".
3. Run `Take Ownership` on the portable MetaTrader 5 directory. I found some settings were not saving otherwise.
4. Run `Port-Trade.Bat` by double clicking it. 
5. Set your stuff up again in MetaTrader 5, it will save for next time if you close MetaTrader 5.
6. When everything Setup (including the EAs you use), back it up, this is now your Master for install purposes.

### NOTATION
- If you want to run multiple accounts on same machine, then duplicate the resulting portable folder.
- If you want a shortcut to the batch, ensure the Target field looks like this `C:\Windows\System32\cmd.exe /c "DRIVE:\PATH TO BATCH\Meta-Port.Bat"`, if you want it on your TaskBar.
- Do not copy across activated EAs from your normal install to the portable directory, this will not work.
- Issues with multi-core now fixed, phew, almost resulted to reinstalling my OS, and even as a last resort installing a beta Motherboard Bios.
  
## DEVELOPMENT
- Use same theme of windows and text as my other batch launchers.

## DISCLAIMER
This software is subject to the terms in License.Txt, covering usage, distribution, and modifications. For full details on your rights and obligations, refer to License.Txt.
