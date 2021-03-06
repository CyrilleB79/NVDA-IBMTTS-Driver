# IBMTTS driver, Add-on for NVDA #
  This add-on implements NVDA compatibility with the IBMTTS synthesizer.
  We can not distribute the IBMTTS libraries. So it is just the driver.
  If you want to improve this driver, feel free to send your pull requests!

# Features:
* Voice, variant, rate, pitch, inflection and volume  setting support.
* Extra head size, Roughness, Breathiness parameters settings support. Create your own voice!
* Enable or disable backquote voice tags. Disable it to protect yourself from malisious codes from jokers, enable it to do many fun things with the synthesizer. Safe fun guaranteed!
* Rate boost. If the synthesizer does not speak very fast to  you, then enable it and get the maximum voice speech!
* auto language changes. Let the synthesizer to read texts in the correct language.
* Indexing support. The cursor will never be lost when using read all feature.
* anti crashing filter expressions. The driver filters known crashing expressions.

# Requirements.
## NVDA.
  You need NVDA 2018.4 or later. This driver is compatible with python 3, So you can use it with future NVDA versions. Once NVDA with python 3 is released, this driver will no longer be compatible with python 2.7. Please use the latest NVDA versions. Its free!

## IBMTTS synthesizer libraries.
  This is just the driver, you must   get the libraries from  somewhere else.

# Installation.
  Just install it as a NVDA add-on. Then open NVDA dialog settings, and set the IBMTTS folder files in the IBMTTS category.
  Also in this category you can copy the external IBMTTS files into Add-on.
  Please note: if the synthesizer is inside the add-on, the driver will update the ini library paths automatically. So you can use it on portable NVDA versions.

# Packaging it for distribution.
  Open a command line, change to the Add-on root folder  and run the scons command. The created add-on, if there were no errors, is placed in the root directory.

## Notes:
* scons and gettext tools on this project are  compatible with python 3 only. Doesn't work with python 2.7.
* You can put the extra IBMTTS required files in the add-on (for personal use only). Just copy them in "addon\synthDrivers\ibmtts" folder. Adjust the default library name in "settingsDB.py" if necessary.