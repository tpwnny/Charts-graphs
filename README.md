

```shell
$ git clone https://github.com/pyecharts/pyecharts.git
$ cd pyecharts
$ pip install -r requirements.txt
$ python setup.py install
```


```python
from pyecharts.charts import Bar
from pyecharts import options as opts

bar = (
    Bar()
    .add_xaxis(["衬衫", "毛衣", "领带", "裤子", "风衣", "高跟鞋", "袜子"])
    .add_yaxis("商家A", [114, 55, 27, 101, 125, 27, 105])
    .add_yaxis("商家B", [57, 134, 137, 129, 145, 60, 49])
    .set_global_opts(title_opts=opts.TitleOpts(title="某商场销售情况"))
)
bar.render()
```
<p align="center">
<img src="https://user-images.githubusercontent.com/19553554/55270272-d6ff1b80-52d7-11e9-820f-30660a068e3e.gif"  width="85%" />
</p>


```python
from pyecharts.render import make_snapshot

# needs to configure selenium
make_snapshot(bar.render(), "bar.png")
```
<p align="center">
<img src="https://user-images.githubusercontent.com/19553554/55270432-7a9cfb80-52d9-11e9-81b5-4ceb4dcd1756.png"  width="85%" />
</p>

### Notebook

#### Jupyter Notebook

![](https://user-images.githubusercontent.com/19553554/55270255-b3d46c00-52d7-11e9-8aa5-f7b3819a1e88.png)

#### JupyterLab

![](https://user-images.githubusercontent.com/19553554/55270259-c0f15b00-52d7-11e9-8811-93bfca1cc027.png)

#### Web framework

![](https://user-images.githubusercontent.com/19553554/35081158-3faa7c34-fc4d-11e7-80c9-2de79371374f.gif)

## 🔖 Demo

<div align="center">
<img src="https://user-images.githubusercontent.com/19553554/52197440-843a5200-289a-11e9-8601-3ce8d945b04a.gif" width="33%" alt="bar"/>
<img src="https://user-images.githubusercontent.com/19553554/52360729-ad640980-2a77-11e9-84e2-feff7e11aea5.gif" width="33%" alt="boxplot"/>
<img src="https://user-images.githubusercontent.com/19553554/52535290-4b611800-2d87-11e9-8bf2-b43a54a3bda8.png" width="33%" alt="effectScatter"/>
<img src="https://user-images.githubusercontent.com/19553554/52332816-ac5eb800-2a36-11e9-8227-3538976f447d.gif" width="33%" alt="funnel"/>
<img src="https://user-images.githubusercontent.com/19553554/52332988-0b243180-2a37-11e9-9db8-eb6b8c86a0de.png" width="33%" alt="gague"/>
<img src="https://user-images.githubusercontent.com/19553554/52344575-133f9980-2a56-11e9-93e0-568e484936ce.gif" width="33%" alt="geo"/>
<img src="https://user-images.githubusercontent.com/19553554/35082102-fd8d884a-fc52-11e7-9e40-5f94098d4493.gif" width="33%" alt="geo"/>
<img src="https://user-images.githubusercontent.com/19553554/52727805-f7f20280-2ff0-11e9-91ab-cd99848e3127.gif" width="33%" alt="graph"/>
<img src="https://user-images.githubusercontent.com/19553554/52345115-6534ef00-2a57-11e9-80cd-9cbfed252139.gif" width="33%" alt="heatmap"/>
<img src="https://user-images.githubusercontent.com/19553554/52345490-4a16af00-2a58-11e9-9b43-7bbc86aa05b6.gif" width="33%" alt="kline"/>
<img src="https://user-images.githubusercontent.com/19553554/52346064-b7770f80-2a59-11e9-9e03-6dae3a8c637d.gif" width="33%" alt="line"/>
<img src="https://user-images.githubusercontent.com/19553554/52347117-248ba480-2a5c-11e9-8402-5a94054dca50.gif" width="33%" alt="liquid"/>
<img src="https://user-images.githubusercontent.com/19553554/52347915-0a52c600-2a5e-11e9-8039-41268238576c.gif" width="33%" alt="map"/>
<img src="https://user-images.githubusercontent.com/19553554/52535013-e48e2f80-2d83-11e9-8886-ac0d2122d6af.png" width="33%" alt="parallel"/>
<img src="https://user-images.githubusercontent.com/19553554/52348202-bb596080-2a5e-11e9-84a7-60732be0743a.gif" width="33%" alt="pie"/>
<img src="https://user-images.githubusercontent.com/19553554/35090457-afc0658e-fc74-11e7-9c58-24c780436287.gif" width="33%" alt="ploar"/>
<img src="https://user-images.githubusercontent.com/19553554/52533994-932b7380-2d76-11e9-93b4-0de3132eb941.gif" width="33%" alt="radar"/>
<img src="https://user-images.githubusercontent.com/19553554/52348431-420e3d80-2a5f-11e9-8cab-7b415592dc77.gif" width="33%" alt="scatter"/>
<img src="https://user-images.githubusercontent.com/19553554/44004598-5636d74e-9e97-11e8-8a5c-92de6278880d.gif" width="33%" alt="tree"/>
<img src="https://user-images.githubusercontent.com/19553554/35082251-b9e23982-fc53-11e7-8341-e7da1842389f.gif" width="33%" alt="treemap"/>
<img src="https://user-images.githubusercontent.com/19553554/52348737-01fb8a80-2a60-11e9-94ac-dacbd7b58811.png" width="33%" alt="wordCloud"/>
<img src="https://user-images.githubusercontent.com/19553554/52433989-4f075b80-2b49-11e9-9979-ef32c2d17c96.gif" width="33%" alt="bar3D"/>
<img src="https://user-images.githubusercontent.com/19553554/52464826-4baab900-2bb7-11e9-8299-776f5ee43670.gif" width="33%" alt="line3D"/>
<img src="https://user-images.githubusercontent.com/19553554/52802261-8d0cfe00-30ba-11e9-8ae7-ae0773770a59.gif" width="33%" alt="sankey"/>
<img src="https://user-images.githubusercontent.com/19553554/52464647-aee81b80-2bb6-11e9-864e-c544392e523a.gif" width="33%" alt="scatter3D"/>
<img src="https://user-images.githubusercontent.com/19553554/52465183-a55fb300-2bb8-11e9-8c10-4519c4e3f758.gif" width="33%" alt="surface3D"/>
<img src="https://user-images.githubusercontent.com/19553554/52798246-7ebae400-30b2-11e9-8489-6c10339c3429.gif" width="33%" alt="themeRiver"/>
<img src="https://user-images.githubusercontent.com/19553554/52349544-c2ce3900-2a61-11e9-82af-28aaaaae0d67.gif" width="33%" alt="overlap"/>
<img src="https://user-images.githubusercontent.com/19553554/35089737-ccc1c01c-fc72-11e7-874d-8ba8b89572eb.png" width="33%" alt="grid"/>
<img src="https://user-images.githubusercontent.com/19553554/35082279-e111743c-fc53-11e7-9362-580160593715.gif" width="33%" alt="timeline"/>
</div>


