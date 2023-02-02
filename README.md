# Event Camera Rotation Dataset (ECRot)
An event camera dataset for rotational motion study

## News

- TODO

## About

The Event Camera Rotation Dataset (ECRot) is an event camera dataset designed for the development of event-based rotational motion related algorithms. ECRot contains totally ten sequences recorded with a DVXplorer (VGA resolution: 640 X 480 pixels) from [iniVation](https://inivation.com/). We provide all sequences in rosbag files that contain events using [dvs_msgs/EventArray](https://github.com/uzh-rpg/rpg_dvs_ros/blob/master/dvs_msgs/msg/EventArray.msg) message types, and IMU data using [sensor_msgs/Imu](http://docs.ros.org/en/api/sensor_msgs/html/msg/Imu.html) message types respectively. The calibration files are provided in yaml files. We generate rotational motion of the event camera in two modes: Motorized mount (7 sequences) and Hand-held (3 sequences). The Motorized mount rotates the event camera approximately in a horizontal plane, while the rotation center still deviates a little from the camera's optical center. For the Hand-held cases, there are some irregular translations. To show the advantages of event cameras over standard cameras, these sequences contain challenging illumination conditions (e.g., looking directly at the sun, reflections in the river and windows) as well as dynamic objects (e.g., moving pedestrians, bicycles, cars, leaves and water on the river).

## Sequences

### Scenes

- Brandenburg Gate
![imagen](images/brandenburg_gate_pano_RGB.jpg)

- Charlottenburg Palace
![imagen](images/charlottenburg_palace_pano_RGB.jpg)

- Victory Column

- TU Berlin Main Building

- TU Berlin MAR Building

- Square Center

- Square Side

- Crossroad

- River

- Bridge

### Description

| Sequence | Camera carrier | Duration [s] | Rotation range [deg] |
| :-----| :-----| ----: | ----: |
| [Brandenburg Gate](https://drive.google.com/drive/folders/1k8C2ngoSKyy9yZOoFwEZWAGs2Utygz5Z?usp=share_link) | Motorized mount | 8.0 | 360 |
| [Charlottenburg Palace](https://drive.google.com/drive/folders/1_1tGqoZB4BnVk4Vt4OnlNTCKV4oXzWw1?usp=share_link) | Motorized mount | 8.4 | 360 |
| [Victory Column](https://drive.google.com/drive/folders/1MbKtWNnaJ_l4iKyW8M0FA6McqKv-X3nc?usp=share_link) | Motorized mount  | 10.0 | 90 |
| [TU Berlin Main Building](https://drive.google.com/drive/folders/1LSo-IyDAQdHpMJwYjzcVXaM6Yms-8X6k?usp=share_link) | Motorized mount | 8.5 | 360 |
| [TU Berlin MAR Building](https://drive.google.com/drive/folders/1uX4DrY5YoCCyEClXmNiE90_fpoZIrED6?usp=share_link) | Motorized mount | 4.0 | $\approx$ 90 |
| [Square Center](https://drive.google.com/drive/folders/18gVBZSuy2qbyLIwg0kNjVy3_1gkuslia?usp=share_link) | Motorized mount  | 8.8 | 360 |
| [Square Side](https://drive.google.com/drive/folders/14hbk54NcUG6uOrsdKqaOzDprQyaxyvNX?usp=share_link) | Motorized mount | 8.0 | 360 |
| [Crossroad](https://drive.google.com/drive/folders/1skZ2LNLBMXbtJaWzy2ijKtlHXYZ9SwAA?usp=share_link) | Hand-held | 10.2 | 360 |
| [River](https://drive.google.com/drive/folders/1USBO6u9tgF-YVMqNABKMDEQwa3peOlH5?usp=share_link) | Hand-held | 5.5 | random |
| [Bridge](https://drive.google.com/drive/folders/1BArPM4voy290iZDDwnoOaBlLZ-YdTQqH?usp=share_link) | Hand-held | 7.5 | random |

### Calibration

- [Motorized mount](https://drive.google.com/file/d/1NqmTqD_S-3Ff0YsgIvEJdnzrZ4Lu0lNy/view?usp=share_link)

- [Hand-held](https://drive.google.com/file/d/1c12Y8s3klhSWhw8D5xvoi7zOqdrMDt4m/view?usp=share_link)

## Publications

- Coming soon...

## License

 - TODO
