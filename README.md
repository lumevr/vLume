# Welcome to *v*LUME!

3D Virtual Reality for Single-Molecule Localization Microscopy



## What is it?

***v*LUME** (Visualization of the Universe in a Micro Environment, pronounced ‘volume’) is a free-for-academic-use immersive **virtual reality-based** (VR) visualization software package purposefully designed to render large **3D-SMLM** data sets (Fig. 1a). It has an intuitive user-interface and is compatible with the major commercial VR hardware, such as the Oculus Rift (S) and HTC Vive. 

*v*LUME accelerates the analysis of highly complex 3D point-cloud data and the rapid identification of defects that are otherwise neglected in global quality metrics. The BioRXiv preprint were we presented this software can be found [here](https://www.biorxiv.org/content/10.1101/2020.01.20.912733v1).

### Key benefits

- **Data Exploration and Comparison**: The configurable user interface allows researchers, without need for programming, to seamlessly switch back-and-forth from a global view of the entire captured sample, to detailed nanoscale views of molecular elements in any arbitrary orientation. The software can be used to leverage the human capacity to quickly interpret local features in these data, such as global and local artefacts (Fig. 1b) that are more difficult to trace by automated software without the ground truth being known. In addition, it is easy to quickly evaluate and compare different processing software, side by side, *e.g*. QuickPALM *vs*. ThunderSTORM (Fig. 1c).

- **Extracting 3D Regions of Interest (RoI) from complex data sets**: Complex biological interactions occur in intricate 3D geometries, with the evaluation of interaction data often requiring the extraction and analysis of specific sub-selections of a data set. To demonstrate this capacity of *v*LUME we carried out complex segmentation tasks where users need to identify and select small local features (tens to hundreds of localizations) in data of large dimensions (millions of localizations; Fig. 1d). A single microtubule can be easily extracted from a complex three-dimensional ‘web’ of microtubules within an eukaryotic cell (see also Fig. 1d).

- **Custom Analysis of user-defined subregions**: Quantitative bioimaging not only relies on high-quality images but quantitative evaluation using bespoke code. Recognising this, we included a user-definable script interpreter written in the multi-paradigm language C#. These data can be easily evaluated to give the user instant quantitative feedback about the specific sub-region of their data set (Fig. 1e). We have included four widely-used analyses (Scripts in C#); Ripley’s K function, Nearest Neighbour, local density and the largest and shortest distances

- **Exporting movies for publications and presentations**: As well as allowing customisation of data for presentation purposes *v*LUME also allows custom waypoints (user angle, pitch and yaw) to be defined simply in the VR environment (Fig. 1a) and to automatically generate a ‘fly-through’ video to allow researchers to articulate their scientific discoveries.

#
![](https://www.biorxiv.org/content/biorxiv/early/2020/01/21/2020.01.20.912733/F1.large.jpg?width=800&height=600&carousel=1)

**Fig. 1** **a)**  *v*LUME rapidly and simply takes large, multidimensional point-cloud datasets from 2D visualization into an immersive 3D VR environment through a systematic workflow: 1) multi-dimensional, SMLM image stacks are processed with any standard fitting algorithms providing multiparameter outputs as .csv or .txt files. 2) The resultant datasets can then be dragged and dropped directly into the *v*LUME software and instantly visualised in virtual reality. 3) By anchoring at user-defined waypoints around these data, a smoothly interpolated fly-through video can be created and exported providing the user with a tool to effectively communicate their discoveries. **b)**  *v*LUME facilitates the 3D, VR visualization of millions of localizations, demonstrated by the super-resolved membrane of a T cell with *v*LUME. The accessible interface enables the user to customize their *v*LUME. The T cell is ~10 μm in diameter and has a isotropic resolution of ~24 nm. (FSA) **c)** Comparative inspection of artifacts introduced into data by localization fitting tools can be quickly performed. This can be seen by comparing localizations of Nuclear Pore Complexes fitted with both QuickPALM and ThunderSTORM algorithms. Scale the NPC of the ~100 nm in diameter, and the nuclear membrane ~20μm in diameter, data is taken over ~200 nm range axial range in z **d)** Selection and isolation of nanoscale, complex biological features can be easily achieved by the user. As examples, a stalk of _a Caulobacter crecentus_ bacterium and a filament of a tubulin network were isolated and a Rol saved for further analysis. The microtubules tangle shows a region of ~ 20 μm × 30 μm (and about 500 nm in depth). The diameter section of a single microtubule is ~40 nm. **e)** Regions of interest can then be analyzed to instantly quantify desired properties using bespoke C# scripts (Ripley’s K, Local Density Plots, Nearest Neighbors and any others).
#

## The software

This **GitHub** repository is where all the official *v*LUME *releases* (https://github.com/lumevr/vLume/releases) will be published. It is free-for-academic-use and the packages include high quality biological samples as well as the latest open-source *plugins* that are under constant development. You can find a specific [repository for the open source plugins here](https://github.com/lumevr/vLume_OpenSourcePlugins). Although the base releases of *v*LUME will be compiled, please feel free to suggest new features, report bugs or start new discussions under the issues tag.

## Some video samples

As a demonstration of the capabilities of *v*LUME we show four videos corresponding to the four key benefits using cutting edge SMLM samples. These and other supplementary videos can be found in the BioRXiv preprint repository.

|                |Link                          |Description                         |
|----------------|---------------------------------|-----------------------------|
|Walk-through     |[Video 1](https://youtu.be/6yx_sayhsiA)           |Overview of the main GUI and functionality in vLUME             |
|Segmentation         |[Video 2](https://youtu.be/J4xSNBVk0wM)             |Demonstration of a user isolating a single microtubule from a complex tangle            |
|Local bespoke analysis          |[Video 3](https://youtu.be/nFNMJE82uMw) |Nearest Neighbour script application to a NPC dataset|
|Exporting features          |[Video 4](https://youtu.be/FAa1C8JPF8o) |Setting waypoints in the 3D space using vLUME and saving these points as a video|
|Loading and Filtering          |[Video 5](https://youtu.be/IRyPPHqAEY8) |Selecting filters to apply to the data in vLume|


## The Community

*v*LUME will, hopefully, nucleate communities of SMLM researchers by facilitating active **collaboration**, development of **bespoke analysis** features (open-source C# plug-ins) and the **sharing** of these tools through two GitHub repositories.

As previously anounced this is first GitHub repository that houses the base program builds ([https://github.com/lumevr/vLume/releases](https://github.com/lumevr/vLume/releases)), through which future revisions of the *v*LUME will be released, with updated additional features and bug fixes. The community is able to suggest improvements and inform the developers of any bugs that they may encounter while running *v*LUME using the default issues report tab in GitHub. In the second repository ([https://github.com/lumevr/vLume_OpenSourcePlugins](https://github.com/lumevr/vLume_OpenSourcePlugins)) is were the community can participate in the  . To sum up:

- The firt repo (this one) is a forum were to discuss about the main features of the **core** package of ***v*LUME** and were bugs and other issues can be reported.

	> Please use the Issues tag below the repo name.
	
- The second repo is were the **open source scripts**, were besides the forum, the people can ans are encouraged to collaborate in improving and adding functionalities to vLUME by cloning and pull requesting (Pull requests tag).

	> Please refer to the README of the Scripts repository for further information.

## How to cite this work

*v*LUME: 3D Virtual Reality for Single-molecule Localization Microscopy

Alexander  Spark,  Alexandre  Kitching,  Daniel  Esteban-Ferrer,  Anoushka  Handa,  Alexander R.  Carr,  Lisa-Maria  Needham,  Aleks  Ponjavic,  Mafalda Da Cunha  Santos,  James  McColl,  Christophe  Leterrier,  Simon J.  Davis,  Ricardo  Henriques,  Steven F.  Lee

bioRxiv 2020.01.20.912733; doi:  https://doi.org/10.1101/2020.01.20.912733

## Contact

- Alexander Kitching (alexandre.kitching@lumevr.com)
- Steve F. Lee (corresponding: sl591 @ cam . ac . uk)
