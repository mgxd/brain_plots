# Brain Plots


#### Installation

```
pip install -e https://github.com/mgxd/brainplot/archive/master.zip --process-dependency-links
```

#### Additional requirements
* X11
* VTK
  * Easiest way to get this is `conda install vtk`
* [Conte69_Atlas](https://github.com/mgxd/brainplot/tree/master/brainplot/Conte69_Atlas)
* [HCP500 Resting Atlas](https://www.dropbox.com/s/avlpaav34bzs6u9/rfMRI_REST1_LR_Atlas.dtseries.nii?dl=0)

##### Arguments [defaults in bold]
  * in_stat, path of statistic to map
  * -o: outfile; **`in_stat`.png**
  * -c: path to Conte69 atlas; **current working directory**
  * -r: path to HCP 500 resting atlas
  * -t: set threshold; **2.3**
  * -s: set image size; 1-smallest, 5-largest; **2**
  * -v: view of the brain: **lat**, sup, or inf
  * -i: inflation level of generated brain mesh: low, **medium**, or high
  * -w: run windowed

##### Sample Use
`git clone` && `cd brainplot/brainplot`

```python
python plotting.py /samples/faces_gt_objects.nii
```
<img src=doc/sample/lateral_split_face_gt_object.png width=500px>
```python
python plotting.py /samples/faces_gt_objects.nii -v inf
```
<img src=doc/sample/inferior_face_gt_object.png width=500px>



##### TODO
[:)](https://github.com/mgxd/brainplot/projects/1)
