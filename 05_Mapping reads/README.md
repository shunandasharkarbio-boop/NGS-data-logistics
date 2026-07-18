BWA-MEM2 on dataset ERR636434
[Link Text](https://usegalaxy.org/api/datasets/f9cad7b01a4721358f0fdf6201b762fd/display)

BWA-MEM2 on dataset ERR636028
[Link Text](https://usegalaxy.org/api/datasets/f9cad7b01a472135fa7b937658b19841/display)

BWA-MEM2 on dataset ERR042232
[Link Text](https://usegalaxy.org/api/datasets/f9cad7b01a4721354572a878f6284b54/display)

BWA-MEM2 on dataset ERR042228
[Link Text](https://usegalaxy.org/api/datasets/f9cad7b01a4721354a49a82a2653e00d/display)


Mapping reads
We can proceed with mapping reads. Galaxy has a number of mappers including bowtie, bwa-mem, and bwa-mem2. For this analysis we will use bwa-mem2 —the latest version of this popular and “battle-tested” tool.

Upload reference genome
The key question when mapping reads against a genome is whether the index for this genome—a datastructure bwa-mem2 uses to quickly find matches—is already installed on Galaxy or not. Let’s assume that it is NOT present in Galaxy. In this case you will need to upload the genome. In this case we will use reference genome of 3D7 strain P. falciparum.
