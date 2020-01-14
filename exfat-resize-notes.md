# Fields from boot region



VolumeLength - size in sectors
FatOffset - offset of FAT in volume
FatLength - each FAT needs space to describe all the clusters in the Cluster Heap
ClusterHeapOffset - start of first cluster
ClusterCount - number of clusters
FirstClusterOfRootDirectory - root dir cluster number
VolumeFlags - VolumeDirty & ActiveFat flags is needed
BytesPerSectorShift & SectorsPerClusterShift - bytes per sector 
PercentInUse - set to 0xFF















