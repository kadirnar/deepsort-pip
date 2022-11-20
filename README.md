<div align="center">
<h2>
  DeepSort-Pip: Packaged version of the DeepSort repository  
</h2>
<h4>
    <img width="500" alt="teaser" src="doc/uav_video.gif">
</h4>
</div>

## <div align="center">Overview</div>

This repo is a packaged version of the [DeepSort](https://github.com/nwojke/deep_sort) algorithm.
### Installation
```
pip install deepsort
```

### Detection Model + DeepSort 
```python
from deepsort.tracker import DeepSortTracker

tracker = DeepSortTracker(args)
for image in images:
   dets = detector(image)
   online_targets = tracker.update(dets)
```
### Citation
```bibtex
@inproceedings{Wojke2017simple,
  title={Simple Online and Realtime Tracking with a Deep Association Metric},
  author={Wojke, Nicolai and Bewley, Alex and Paulus, Dietrich},
  booktitle={2017 IEEE International Conference on Image Processing (ICIP)},
  year={2017},
  pages={3645--3649},
  organization={IEEE},
  doi={10.1109/ICIP.2017.8296962}
}

@inproceedings{Wojke2018deep,
  title={Deep Cosine Metric Learning for Person Re-identification},
  author={Wojke, Nicolai and Bewley, Alex},
  booktitle={2018 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  year={2018},
  pages={748--756},
  organization={IEEE},
  doi={10.1109/WACV.2018.00087}
}
```
