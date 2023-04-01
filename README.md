# Iterative Closest-Point (ICP)
The Iterative Closest-Point (ICP) algorithm is a point cloud registration algorithm widely used in robotics and computer vision to estimate the rigid transformation between two point clouds. It is capable of finding a transformation that minimizes the distance between the points of one cloud and the corresponding points in the other cloud.

The ICP works by finding point correspondences between the two point clouds and then applying a transformation to minimize the distance between the correspondences. The process is iterated until the transformation converges to an optimal value.

# Using ICP to estimate the trajectory of a car using LiDAR sensor point cloud
ICP can be used to estimate the trajectory of a car using LiDAR sensor point cloud. In this case, the point cloud represents the points of the environment around the car. Using ICP, it is possible to estimate the rigid transformation between the current point cloud and the previous point cloud. With this information, the car trajectory can be estimated.

To use ICP, it is necessary to collect point clouds continuously using the LiDAR sensor. Then, the algorithm is applied to estimate the rigid transformation between the point clouds. The car trajectory can be estimated from the rigid transformation found.

The proposed solution involves using a set of 30 scans obtained from a LiDAR sensor, which are part of the KITTI DATASET. With this data, the goal is to estimate the trajectory traveled by the car. To achieve this, a custom algorithm is implemented, without using third-party libraries. At the end of the process, the path traveled by the car is displayed in all axes (XYZ).
