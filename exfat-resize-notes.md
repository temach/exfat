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









Useful links:
    - Specification: https://github.com/MicrosoftDocs/win32/blob/docs/desktop-src/FileIO/exfat-specification.md
    - Directory structure description: http://www.ntfs.com/exfat-directory-structure.htm
    - Simple FAT explained: https://www.pjrc.com/tech/8051/ide/fat32.html
    - Testing the filesystem 1: https://serverfault.com/questions/19487/how-to-do-filesystem-testing
    - Testing the filesystem 2: https://stackoverflow.com/questions/21565865/filesystem-test-suites





