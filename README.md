## TopoInput: TopoBuilder Input PyMOL Plugin


#### Requirements

PyMOL 2.x

Python 2.7

TopoBuilder v1.0.2


#### Install

1）TopoBuilder

Open Conda-Prompt.bat under PyMOL installation directory

(make sure the python version of conda with PyMOL is 2.7)

```Bash
pip install https://github.com/lpdi-epfl/topobuilder/archive/v1.0.2.zip
```

2）TopoInput Plugin

Install with PyMOL's plugin manager:

Plugin > Plugin Manger > Install New Plugin > Install from local file

Simply choose the TopoInput.zip


#### Usage

1）Set the working directory of PyMOL

* File > Working Directory > Change...

(the PDB file of insertion motif should be here)

2）Open TopoInput plugin

* Plugin > TopoInput

3）Write the input scripts

- config：name, fragment file path and Rosetta path
- layers：the topology of ideal protein sketch
- motifs：the insertion functional motif (from original PDB)

Detailed introduction of parameters can be found [here](https://github.com/LPDI-EPFL/topobuilder/tree/releasepy2).

4）Click the 'Show Sketch' button

Defined protein shapesketch will show in PyMOL window.

If you are not satisfied with the shown shapesketch, you can adjust the parameters in the script then click the Show Sketch button again.

5）Click the 'Build All' button

The entire output files of TopoBuilder will appear in working directory, including all connection ways of this sketch.


#### To Do

More interactive dialog for designing simple scaffolds

Python 3 version for new TopoBuilder



#### References

[PyMOL Demo Plugin](https://github.com/Pymol-Scripts/pymol2-demo-plugin)

[TopoBuilder v1.0.2](https://github.com/LPDI-EPFL/topobuilder/tree/releasepy2)
