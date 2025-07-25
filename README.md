# PythonPart DesignAndModelingTools
The PythonPart contains a set of tools to improve design and modeling workflows within Allplan:
- **Creat3DfromArea** to convert area elements to 3D
- **DrawBodyOnPlane** to create projections of 3D bodies on a plane
- **FlattenCurves** to convert 3D curves to 2D
- **PolygonizeArea** to draw a border around area elements
- **ProjectOnPlan** to create projections of 3D curves on a plane

As each of them is a single PythonPart itself they can be executed and used independend from each other.

## Installation
The PythonPart **DesignAndModelingTools** can be installed directly from the Plugin Manager in ALLPLAN. 

Alternatively, the corresponding ***.allep** package can be downloaded from the [release page](https://github.com/AnkeNiedermaier/design-modeling-tools-public/releases). ***.allep** files are ALLPLAN internal setups that can be installed via drag and drop into the program window.

At least the version 2026 is needed to install the PythonPart.

## Installed PythonPart Scripts
If the installation was successfull, the individual PythonParts **Creat3DfromArea.pyp**, **DrawBodyOnPlane.pyp**, **FlattenCurves.pyp**, **PolygonizeArea.pyp** and **ProjectOnPlan.pyp** can be found
in the ALLPLAN Library:
`Office` → `ALLPLAN GmbH` → `DesignAndModelingTools`\
Besides this, they are also added to the ActionBar in a new created task area **DesignAndModelingTools** in the tasl Plug-ins.

# Workflow
Although the single PythonParts cover different use-cases, the structure of the corresponding palette is more or less the same. They all contain the sections:
- **Object selection**
- **Format**
- **Creation**

and the **..OnPlane** PythonParts additionally one for the **Plane definition**.\
For the latter the definition of a plane is necessary first, whereas for the others the palette content is shown directly when the PythonPart is started.

## Plane definition
To specify the plane on which the objects should be projected, the PythonParts **DrawBodyOnPlane** and **ProjectOnPlane** reqiure the input of 3 points as stated in the dialog line
