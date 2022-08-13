# shared-functions

Repository of shared, relatively self-contained functions that can be re-used across missions.

## Usage

Using the shared functions is relatively easy:

1. Copy or merge the `CfgFunctions` class from the `description.ext` into your own mission's `descrition.ext`.
2. Copy the `Functions\` directory (and sub directories) into the root of your mission folder.
   1. You MUST keep the structure as-is, otherwise you will have to edit the CfgFunctions to point to a new location.
3. (OPTIONAL) If you are desperate to save space, you can delete the function files `fn_*` that you are not using. But be sure to remove their reference from your `CfgFunctions` too!

## Contributing

Adding a function to this is two steps:

1. To add a function, simply copy the SQF file into a category folder under `Functions` and ensure the filename is prefixed with `fn_`.
   1. Feel free to create a new category folder if one doesn't exist that matches your function usage.
2. Update the `description.ext`, adding a new subclass under `CfgFunctions` with your TAG and then any other subclasses for the category.
   1. This is prefixed on the global variable for your function, for example `TAG_fnc_functionName`.
   2. If using a category subclass, it must match the folder structure.

```cpp
class CfgFunctions
{
   class MYTAG {
      class General {
         // Corresponds to Functions\General\fn_doThing.sqf
         class doThing {};
      };
   };
};
```

## References

For more information on `CfgFunctions`, see the [Arma 3 wiki](https://community.bistudio.com/wiki/Arma_3:_Functions_Library).
