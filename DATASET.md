## DATASET
The following is adapted from [Danfei Xu](https://github.com/danfeiX/scene-graph-TF-release/blob/master/data_tools/README.md) and [neural-motifs](https://github.com/rowanz/neural-motifs).

### Download:
1. Download the VG images [part1 (9 Gb)](https://cs.stanford.edu/people/rak248/VG_100K_2/images.zip) [part2 (5 Gb)](https://cs.stanford.edu/people/rak248/VG_100K_2/images2.zip). Extract these images to the file `datasets/vg/VG_100K`. If you want to use other directory, please link it in `DATASETS['VG_stanford_filtered']['img_dir']` of `maskrcnn_benchmark/config/paths_catelog.py`. 
2. Download the [scene graphs labels](https://onedrive.live.com/embed?cid=22376FFAD72C4B64&resid=22376FFAD72C4B64%21779871&authkey=AA33n7BRpB1xa3I) and extract them to `datasets/vg/VG-SGG-with-attri.h5`, or you can edit the path in `DATASETS['VG_stanford_filtered_with_attribute']['roidb_file']` of `maskrcnn_benchmark/config/paths_catalog.py`.
3. Download the [detection results](https://drive.google.com/drive/folders/1SdMXwXpdTZdxYOZl0OcPqqGd2p4DhePt?usp=sharing) of 3 datasets, including: Conceptual Caption, COCO Caption and Visual Genome. After downloading, you can run `cat cc_detection_results.zip.part* > cc_detection_results.zip` to merge several partitions into one zip file and unzip it to folder `datasets/vg/`.
4. Download the [extracted caption label files](https://drive.google.com/drive/folders/1EX60amQYbeiXfZX-RN2hAdlHBCdwhc-_?usp=sharing) for COCO and VG dataset and save them in the folder `datasets/caption_labels`.


### Folder structure:
After downloading the above files, you should have following hierarchy in folder `datasets/vg/`:

```
├── VG_100K
├── cc_detection_results_oid
├── COCO_detection_results_oid
├── VG_detection_results_oid
└── VG-SGG-with-attri.h5
```

