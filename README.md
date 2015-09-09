# ACAD-LayOrd
Re-order your AutoCAD drawings while working on them or at plot/print time with a few simple clicks.

This will solve problems with bad draw order by the user when working, or issues where a hatch bleeds over a fine line weight, etc.

## Installation
Edit your existing acad.lsp file to include the .lsp in this package, or create yourself a new one with the below:
```
(defun s::startup ()
(load "layord.lsp")
)
```
Then place the acad.lsp in your chosen AutoCAD file search path.

Place the layord.lsp in your chosen AutoCAD file search path.

Not sure where you should put it? Example:
```
C:\Program Files\Autodesk\AutoCAD 2015
```
```
C:\Program Files\Autodesk\AutoCAD 2015\Acade
```
If you have trouble, read the AutoCAD documentation for where to put these files. ```DSETTINGS``` will allow you to check your current paths.

Optionally, you can place the layord.lsp anywhere and load it via drop and drag, or menu for each drawing you wish to use it on.

An acad.lsp is included in the package for convenience for new users.

## Usage
The AutoCAD command to run is ```layord```.
This will bring up the dialog.

The interface itself is self explanatory. You have your non-XRef layers on the left to choose from and can shift them to the right hand side for re-ordering with the arrow.

The arrows on the right hand side re-order the layers in the list, and the move button at the bottom initiate the re-ordering.

If you need help use the help button.
