# MORAI_Simulator
MORAI Simulator 프로젝트 소스코드입니다.

## Environment Setting
|OS|Version|
|:---:|:---:|
|Ubuntu|18.04|
|ROS|Melodic|

## Camera
코드에 대한 자세한 내용은 [여기](camera_gps/README.md)를 참고해 주시길 바랍니다.

<details>
<summary>1. sub_camera.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/9a1d70af-1a90-4de3-b162-1e205c62273f" width="60%" height="60%" title="1. sub_camera.py"></p>


```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 1.sub_camera.py 
```

</details>

<details>
<summary>2. pub_camera.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/3b44d0fe-1dea-411e-b31d-571ecc57a86f" width="60%" height="60%" title="2. pub_camera.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 2.pub_camera.py 
```

</details>

<details>
<summary>3. bird_eye_view.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/1adb95dc-ccc8-41cf-b09f-2a6efc4e768f" width="60%" height="60%" title="3. bird_eye_view.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 3.bird_eye_view.py 
```

</details>

<details>
<summary>4. white_line_detect.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/076c7b22-f1fd-4211-95c0-ac8771cdada0" width="60%" height="60%" title="4. white_line_detect.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 4.white_line_detect.py 
```

</details>

<details>
<summary>5. yellow_line_detect.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/72e87e54-b45b-4d48-b325-d42d1608d8bf" width="60%" height="60%" title="5. yellow_line_detect.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 5.yellow_line_detect.py 
```

</details>

<details>
<summary>6. blend_line.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/2f81476d-18f0-40ca-b1c7-36c75d1bf381" width="60%" height="60%" title="6. blend_line.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 6.blend_line.py 
```

</details>

<details>
<summary>7. binary_line.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/0a986f04-44dd-4674-bab4-8fcf9e77d9c3" width="60%" height="60%" title="7. binary_line.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 7.binary_line.py 
```

</details>

<details>
<summary>8. sliding_window.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/896efc26-0d98-4047-b3df-1823f5ba65a5" width="60%" height="60%" title="8. sliding_window.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 8.sliding_window.py 
```

</details>

<details>
<summary>9. LAKS.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/e9b52321-8216-4c20-890c-81f43d9c1af5" width="60%" height="60%" title="9. LAKS.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
rosrun scout_ros 9.LAKS.py 
```

</details>

## GPS
코드에 대한 자세한 내용은 [여기](camera_gps/README.md)를 참고해 주시길 바랍니다.

<details>
<summary>path_maker.launch </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/9e4973de-3d70-4510-b733-c7a1b048b71e" width="60%" height="60%" title="path_maker.launch"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
roslaunch scout_ros path_maker.launch 
```

</details>

<details>
<summary>planner.launch </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/6011e374-c0d7-4989-b782-c0d04d7fa588" width="60%" height="60%" title="planner.launch"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
roslaunch scout_ros planner.launch
```

</details>

## SLAM
코드에 대한 자세한 내용은 [여기](slam_navigation/README.md)를 참고해 주시길 바랍니다.

<details>
<summary>slam_gmapping_pr2.launch </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/3ae3fcba-dcf6-426c-b670-0b69243c6a95" width="60%" height="60%" title="slam_gmapping_pr2.launch"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
roslaunch kw_tf tf_setting.launch
roslaunch pointcloud_to_laserscan sample_node.launch
roslaunch gmapping slam_gmapping_pr2.launch
```
<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/105b5791-0142-48d3-ac6e-e2abf04cbe77" width="60%" height="60%" title="map"></img><br/></p>

```python
rosrun map_server map_saver
```

</details>

## Navigation
코드에 대한 자세한 내용은 [여기](slam_navigation/README.md)를 참고해 주시길 바랍니다.

<details>
<summary> navigation.launch </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/ef0ab727-3bc3-47e4-a936-5b2ebdead674" width="60%" height="60%" title="navigation.launch"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
roslaunch kw_tf tf_setting.launch
roslaunch pointcloud_to_laserscan sample_node.launch
roslaunch kw_tf navigation.launch
```

</details>

<details>
<summary> application.py </summary>

<p align="center"><img src="https://github.com/ehdxns/MORAI_PROJECT/assets/129836561/39e1c14e-cdbe-4ef6-81e1-9b57d370e436" width="60%" height="60%" title="application.py"></p>

```python
roslaunch rosbridge_server rosbridge_websocket.launch
roslaunch kw_tf tf_setting.launch
roslaunch pointcloud_to_laserscan sample_node.launch
roslaunch kw_tf navigation.launch
```

```python
python application.py
```

</details>
