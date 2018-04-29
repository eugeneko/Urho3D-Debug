# Urho3D-Debug

## Overview

This is debug visualizer of Urho3D types.

Requires Visual Studio 2015 or later.

Might work unstable if Urho3D is linked dynamically (`URHO3D_LIB_TYPE=SHARED`).

### StringHash debugging

`URHO3D_HASH_DEBUG` option should be on.

To enable `StringHash` reversing in Visual Studio with **dynamically** linked Urho3D library (`URHO3D_LIB_TYPE=SHARED`), add the following snippet somewhere in the executable module.

```
namespace Urho3D
{
    const StringMap* hashReverseMap = StringHash::GetHashReverseMap();
}
```

## How to install

Put `Urho3D.natvis` into Visual Studio 2015 folder

`C:/Users/(username)/Documents/Visual Studio 2015/Visualizers`

or add it to your project like source file.
