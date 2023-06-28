[![Simulation](../../actions/workflows/main.yml/badge.svg)](../../actions/workflows/main.yml)

# Lesson 8 - Exporting Data

The [`tape`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module&doc=/Module/Tape.md) module [`recorder`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module/Tape&doc=/Module/Tape/Recorder.md) object is used to record data from an object. The object must specify the file name, the sampling interval, and the object properties to be sampled.  

The `tape` module can output CSV files with a single header line using the [`csv_header_type`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module/Tape/Global&doc=/Module/Tape/Global/Csv_header_type.md) module variable using the `NAME` option.

Output data can be plotted using the [`plot`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Subcommand&doc=/Subcommand/Plot.md) subcommand. The `plot` is run when the simulation exits successfully with exit code `0` using the [`#on_exit`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/GLM/Macro&doc=/GLM/Macro/On_exit.md) macro. 

## Tasks

1. Setup the building schedule (see [`main.glm@6`](main.glm#L6-L14)).
2. Import the `tape` module (see [`main.glm@16`](main.glm#L17-L20)).
3. Add the commercial building to `load_1` (see [`main.glm@22`](main.glm#L23-L52)).
4. Add the data recorder to the building (see [`main.glm@45`](main.glm#L46-L51)).
5. Get and load the weather forecast (see [`main.glm@54`](main.glm#L55-L56)).
6. Set the simulation clock (see [`main.glm@58`](main.glm#L59-L64)).
7. Plot the load when the simulation exits successfully (see [`main.glm@66`](main.glm#L67)).

# Exercices

1. Plot the load of a residential building on load 2.

# More Information

* [Tape module](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module&doc=/Module/Tape.md)
* [Recorder object](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module/Tape&doc=/Module/Tape/Recorder.md)

# Next Lesson

* [Lesson 9 - Importing Data](../../../lesson-9)
