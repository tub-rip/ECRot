# Event Camera Rotation Dataset (ECRot)
The Event Camera Rotation Dataset (ECRot) is a VGA-resolution event camera dataset designed for the development of event-based rotational motion related algorithms. ECRot contains ten sequences recorded with a DVXplorer (640 x 480 pixels) from [iniVation](https://inivation.com/). We provide all sequences in ROSbag files that contain events using [dvs_msgs/EventArray](https://github.com/uzh-rpg/rpg_dvs_ros/blob/master/dvs_msgs/msg/EventArray.msg) message types, and IMU data using [sensor_msgs/Imu](http://docs.ros.org/en/api/sensor_msgs/html/msg/Imu.html) message types respectively. The camera calibration files are provided in yaml files.

Rotational motion is generated in two modes: Motorized mount (7 sequences) and Hand-held (3 sequences). The motorized mount rotates the event camera approximately around its vertical axis, while the rotation center slightly deviates from the camera's optical center. In the hand-held sequences, there are also some minor unavoidable translations. To show the advantages of event cameras over standard cameras, these sequences contain challenging illumination conditions (e.g., looking directly at the sun, reflections in the river and windows) as well as dynamic objects (e.g., moving pedestrians, bicycles, cars, leaves and water on the river).

<!-- An event camera dataset for rotational motion study

## News

- TODO -->


## Sequences

### Description

| Sequence | Setup | Duration [s] | Rotation range [deg] | File size |
| :-----| :-----| ----: | ----: | ----: |
| [Brandenburg Gate](https://drive.google.com/drive/folders/1k8C2ngoSKyy9yZOoFwEZWAGs2Utygz5Z?usp=share_link) | Motorized mount | 8.0 | 360 | 1.40 GB |
| [Charlottenburg Palace](https://drive.google.com/drive/folders/1_1tGqoZB4BnVk4Vt4OnlNTCKV4oXzWw1?usp=share_link) | Motorized mount | 8.4 | 360 | 1.18 GB |
| [Victory Column](https://drive.google.com/drive/folders/1MbKtWNnaJ_l4iKyW8M0FA6McqKv-X3nc?usp=share_link) | Motorized mount  | 10.0 | 90 | 62.2 MB |
| [TU Berlin Main Building](https://drive.google.com/drive/folders/1LSo-IyDAQdHpMJwYjzcVXaM6Yms-8X6k?usp=share_link) | Motorized mount | 8.5 | 360 | 1.41 GB |
| [TU Berlin MAR Building](https://drive.google.com/drive/folders/1uX4DrY5YoCCyEClXmNiE90_fpoZIrED6?usp=share_link) | Motorized mount | 4.0 | $\approx$ 90 | 421 MB |
| [Square Center](https://drive.google.com/drive/folders/18gVBZSuy2qbyLIwg0kNjVy3_1gkuslia?usp=share_link) | Motorized mount  | 8.8 | 360 | 1.37 GB |
| [Square Side](https://drive.google.com/drive/folders/14hbk54NcUG6uOrsdKqaOzDprQyaxyvNX?usp=share_link) | Motorized mount | 8.0 | 360 | 1.46 GB |
| [Crossroad](https://drive.google.com/file/d/1misnorq_iyK-uMfZWadDMu0RxF10dMN9/view?usp=share_link) | Hand-held | 10.2 | 360 | 792 MB |
| [River](https://drive.google.com/drive/folders/1USBO6u9tgF-YVMqNABKMDEQwa3peOlH5?usp=share_link) | Hand-held | 5.5 | random | 862 MB |
| [Bridge](https://drive.google.com/drive/folders/1BArPM4voy290iZDDwnoOaBlLZ-YdTQqH?usp=share_link) | Hand-held | 7.5 | random | 1.08 GB |

### Intrinsic calibration of the event camera:

- [Motorized mount](https://drive.google.com/file/d/1NqmTqD_S-3Ff0YsgIvEJdnzrZ4Lu0lNy/view?usp=share_link)

- [Hand-held](https://drive.google.com/file/d/1c12Y8s3klhSWhw8D5xvoi7zOqdrMDt4m/view?usp=share_link)

### Scenes (from an RGB frame-based camera)

The panoramas captured by an iPhone 11 and the panoramic Images of Warped Events (IWEs) produced by CMax-SLAM are presented as below.

- [Brandenburg Gate](https://en.wikipedia.org/wiki/Brandenburg_Gate)
![gate_rgb_pano](images/panoramas/brandenburg_gate.jpg)
![imagen](images/exp_map/gate_pano_IWE_expscale-100.png)

- [Charlottenburg Palace](https://de.wikipedia.org/wiki/Schloss_Charlottenburg)
![imagen](images/panoramas/charlottenburg_palace.jpg)
![imagen](images/exp_map/palace_pano_IWE_expscale-100.png)

- [Victory Column](https://en.wikipedia.org/wiki/Berlin_Victory_Column)
![imagen](images/panoramas/victory_column.jpg)
![imagen](images/exp_map/victory_column_0-3.9_-30_exp_30.png)

- TU Berlin Main Building
![imagen](images/panoramas/tub_main_building.jpg)
![imagen](images/exp_map/main_building_pano_IWE_expscale-100.png)

- TU Berlin MAR Building
![imagen](images/panoramas/tub_mar_building.jpg)
![imagen](images/exp_map/mar_building_0-3.8_-30_exp_50.png)

- Square Center
![imagen](images/panoramas/square_center.jpg)
![imagen](images/exp_map/square_center_0-8_-90_exp_100.png)

- Square Side
![imagen](images/panoramas/square_side.jpg)
![imagen](images/exp_map/square_side_0-7.5_-90_exp_100.png)

- Crossroad
![imagen](images/panoramas/crossroad.jpg)
![imagen](images/exp_map/crossroad_pano_IWE_expscale-100.png)

- River
![imagen](images/panoramas/river.jpg)
![imagen](images/exp_map/river_0-5_0_exp_100.png)

- Bridge
![imagen](images/panoramas/bridge.jpg)
![imagen](images/exp_map/bridge_0-7_0_exp_100.png)

## Acknowledgements
Ms. Nan Cai (for assistance on the motorized sequences) and Mr. Yunfan Yang (for assistance with the hand-held sequences).

## Citation

```bibtex
@Article{Guo24tro,
  author        = {Shuang Guo and Guillermo Gallego},
  title         = {{CMax}-{SLAM}: Event-based Rotational-Motion Bundle Adjustment and {SLAM} System using Contrast Maximization},
  journal       = tro,
  year          = 2024,
  volume        = {},
  number        = {},
  pages         = {1--20}
}
```

## License

- Coming soon...
