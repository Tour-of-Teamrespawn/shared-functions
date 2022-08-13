# shared-functions

Repository of shared, relatively self-contained functions that can be re-used across missions.

## Usage

Using the shared functions is relatively easy:

1. Copy or merge the `CfgFunctions` class from the `description.ext` into your own mission's `descrition.ext`.
2. Copy the `Functions\` directory (and sub directories) into the root of your mission folder.
   1. You MUST keep the structure as-is, otherwise you will have to edit the CfgFunctions to point to a new location.
3. (OPTIONAL) If you are desperate to save space, you can delete the function files `fn_*` that you are not using. But be sure to remove their reference from your `CfgFunctions` too!

For more information on `CfgFunctions`, see the [Arma 3 wiki](https://community.bistudio.com/wiki/Arma_3:_Functions_Library).
