---
layout: about
title: About
permalink: /
# subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Moto. Etc.

profile:
  align: right
  image: profile-pic.jpg
  # address: >
  #   <p>555 your office number</p>
  #   <p>123 your address street</p>
  #   <p>Your City, State 12345</p>

# news: true  # includes a list of news items
# selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

<!-- Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com). You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](http://fortawesome.github.io/Font-Awesome/) and [Academicons](https://jpswalsh.github.io/academicons/), like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them. -->

Hi there, I'm a robotics software engineer, graduating from CMU in May 2022. Here's a brief self-intro. 

On the tech side, I'm enthusiastic about every technology to bridge the virtual and the real world. Robotics is all about that. Although most of my current interests stay with SLAM, geometry, and 3D vision, I won't resist learning and practicing on any other robotics topic. 

As for my personality, I'm always fascinated by the opportunities to build systems from scratch and witness the real applications. I love challenges and I believe one of the meanings of life come from the efforts to challenge our limits. Every time I step out of my comfort zone, my knowledge and capability expand significantly.

<!-- <p align="center">
  {% include social.html %}
</p> -->

<br>

---

<br>

# Projects

## Digital Twin: An Open Source Solution

*I did this project mainly for fun. NeRF is quite capable, and only needs a camera, but the objects in NeRF are not arbitrarily deformable after training. Meanwhile, many AI body pose estimators are available online, requiring only a camera as well. Blender is a free and open-source 3D modeling software. So my question was: can we combine them together? Now the answer is "Yes!"*

- Created my own digital twin with a cellphone camera and some open-source software
- Calibrated my camera, took body pictures, estimated camera poses in COLMAP, and trained a NeRF model
- Cleaned, simplified and smoothed the mesh extracted from NeRF in Blender
- Built pose bones and assigned the corresponding patches of the mesh in Blender
- Extracted target body poses from an online dancing video using MediaPipe, and animated my digital twin to imitate the dancing gestures

<p align="center">
  <iframe
      src="https://www.youtube.com/embed/NvI3KYCf9A0"
      width="480"
      height="360"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</p>

[Source Code](https://github.com/YukunXia/Digital-Twin-An-Open-Source-Solution)

## An Empirical Study on Multi-View Reconstruction Methods

Mar 2022 - Apr 2022

Collaborator: Yuqing Qin

- Course project for 16-889 "Learning for 3D Vision"
- Quantitatively and qualitatively compared dense multi-view reconstruction quality of COLMAP, MVSNet and NeRF in customized challenging scenes
- Stored some of our CMU memories into neural represented 3D worlds
  - "DD Arm" locates on the 4th floor of Newell-Simon Hall, next to the bridge to Wean Hall
  - "Lion" records one of the two lion statues on [1060 Morewood Ave](https://www.google.com/maps/@40.4450345,-79.942756,3a,75y,104.06h,87.19t/data=!3m6!1e1!3m4!1sNjAJIfiUBCsCBmWH6BnnBA!2e0!7i16384!8i8192). Many people know that the fence is regularly repainted, but these two lions change their appearances very often as well.


<p align="center">
    <img src="/assets/img/projects/multi-view-reconstruction-methods-00.png" width="500">
    <figcaption align = "center">
      <b> Sample results in the first three scenes </b>
    </figcaption>
</p>

[Report PDF](https://drive.google.com/file/d/1mGUzMCABiEHSW0bTtk_dl6TKVJk_pyuT/view?usp=sharing)


## Autonomous Mapping and Exploration in a Simulated Farmland

Mar 2022 - Apr 2022

Collaborator: Calen Robinson

- Course project for 16765-A "Special Topics: Robotics & AI for Agriculture"
- Built a farmland simulation environment and tested autonomous exploration with a Clearpath Husky robot and a 3D lidar
- Implemented the frontier detection algorithm to determine the next best goal
- Implemented and optimized the pure pursuit algorithm to enable agile motions and faster failure recovery
- Used Octomap to store the 3D map and extract the 2D occupancy grid
- Compared the exploration efficiency of different lidar configurations

<p align="center">
    <img src="/assets/img/projects/farmland-exploration-00.png" width="600">
    <figcaption align = "center">
      <b> Our final project poster </b>
    </figcaption>
</p>

<p align="center">
  <iframe
      src="https://www.youtube.com/embed/yeF6xDfmzNk"
      width="480"
      height="360"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</p>

[Source Code](https://github.com/YukunXia/Farmland-Exploration)


## Deployment of SuperPoint on Jetson Nano

Oct 2021 - Dec 2021

Collaborator: Yuqing Qin

- Course project for 11-767 "On-Device Machine Learning"
- Retrained SuperPoint models with different configurations, deployed them on a Jetson Nano
- Tested the trade-off between performance and energy efficiency on the KITTI dataset

<p align="center">
    <img src="/assets/img/projects/superpoint-00.png" width="400">
    <figcaption align = "center">
      <b> System diagram </b>
    </figcaption>
</p>

<p align="center">
    <img src="/assets/img/projects/superpoint-01.png" width="500">
    <figcaption align = "center">
      <b> One of our superpoint models tracking interframe keypoint motions in the KITTI dataset </b>
    </figcaption>
</p>

[Source Code](https://github.com/YukunXia/SuperPoint-Stereo-Visual-Odometry)

[Report PDF](https://github.com/YukunXia/SuperPoint-Stereo-Visual-Odometry/blob/test_two_batches/ODML_project_report.pdf)


## Mobile Robot Object Classiﬁcation & Avoidance

Oct 2020 - Nov 2021

Collaborator: Calen Robinson, Gitaek Lee, Jinkun Liu, Thomas Xu 

- This is a team capstone project, sponsored by Omron Robotics
- Conducted Agile teamwork and developed ROS programs in C++
- Built a factory simulation environment in Gazebo with mobile robots, forklifts and pedestrians
- Trained YOLOv5 and deployed the model onto Jetson AGX Xavier via TensorRT, reaching 50FPS
- Calibrated camera-lidar-robot extrinsics with nonlinear least square solvers
- Estimated object locations by fusing image object detection and lidar point cloud
- Set up a ground truth system to evaluate the performance of object detection models and the sensor fusion algorithm

[Website](https://mrsdprojects.ri.cmu.edu/2021teamd/)

## Reimplementation of V-LOAM

Mar 2021 - May 2021

Collaborator: Ivan Cisneros, Shuqin Xie, Xinjie Yao

- Course project for 16-833 "Robot Localization and Mapping"
- Extracted and matched features from images; estimated continuous depth map from point cloud; optimized frame-to-frame motion with Ceres
- Refactored A-LOAM to integrate with visual odometry and enabled more controllable intermodular communication
- Reduced translation and rotation error of A-LOAM respectively by 26.9% and 22.5% in 9 KITTI sequences in average

<p align="center">
  <iframe
      src="https://www.youtube.com/embed/NnoxB3r_cDM"
      width="480"
      height="360"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</p>

[Source Code](https://github.com/YukunXia/VLOAM-CMU-16833)

[Report PDF](https://github.com/YukunXia/VLOAM-CMU-16833/blob/master/16833_report_V2.pdf)

## Dense SLAM with Point-Based Fusion

Apr 2021 - Apr 2021

- One of the assignments of 16-833 "Robot Localization and Mapping". *Its scale is not as large as other projects here, but the topic is pretty relevant*
- Used projective data association between RGBD frames for fast ICP, and reconstructed dense map through local point fusion
- The dataset is ICL-NUIM

<p align="center">
    <img src="/assets/img/projects/dense-slam-00.png" width="500">
    <figcaption align = "center">
      <b> A reconstructed scene</b>
    </figcaption>
</p>

## Autonomous Exploration Development Environment

Sept 2020 - January 2021

Independent Study Advised by Ji Zhang

- Built a dense resonctruction of CMU campus to test robot exploration algorithms
- Refined simulation environments in Blender
- Wrote a literature review for multiple robot exploration


<p align="center">
    <img src="/assets/img/projects/ground-based-autonomy-00.png" width="500">
    <figcaption align = "center">
      <b> The reconstructed CMU campus</b>
    </figcaption>
</p>

[Project Website](https://www.cmu-exploration.com/)

## Real-time MPC with iLQR for Self-Driving in Carla

Apr 2020 - Jun 2020

- Learned the vehicle dynamical model by combining the bicycle model and neural network
- Implemented the iLQR algorithm from scratch with Google Jax
- Leveraged the log-sum-exp trick to approximate the true distance function in the waypoint following task, avoiding deviations at the sharp turn.
- Validated the real-time performance of MPC algorithm in Carla, with iLQR potentially running in 1kHz

<p align="center">
  <iframe
      src="https://www.youtube.com/embed/AEuxxsT1zcI"
      width="480"
      height="360"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</p>

[Source Code](https://github.com/YukunXia/Carla_iLQR_MPC)

## LQR Funnel Graph for Kinodynamic Planning

Mar 2020 - May 2020

- Course project for 6.832 "Underactuated Robotics"
- Generated trajectories in the state space of a single pendulum through trajectory optimization
- Used Sum-of-Square Programming to calculate the region of attraction (RoA) along the trajectories, in the shape of funnels
- Practiced the kinodynamic planning through Depth First Search on the precomputed funnel graph

<p align="center">
  <iframe
      src="https://www.youtube.com/embed/MIZTSZ0CJZA"
      width="480"
      height="360"
      frameborder="0"
      allowfullscreen="">
  </iframe>
</p>

<br>

---

<br>