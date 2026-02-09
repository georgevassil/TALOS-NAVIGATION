# TALOS-NAVIGATION

αφοτου φτιαξω το docker και ακολουθησω τα βηματ γκιτχαμπ κανω αυτο για να κατεβουν τα packages δεν χρειαζεται μετα build απλως source devel/setup.bash
```bash
apt-get update
apt-get install -y \
    ros-noetic-slam-gmapping \
    ros-noetic-map-server \
    ros-noetic-amcl \
    ros-noetic-move-base \
    ros-noetic-teleop-twist-keyboard \
    ros-noetic-urdf-geometry-parser \
    ros-noetic-effort-controllers \
    ros-noetic-joint-state-controller
apt-get install -y ros-noetic-teb-local-planner

```

αφου αποθηκευσω το μαπ (κατι το οποιο δεν χρειαζεται δνε το χρησιμοποιοθμε υπαρει ηδη ενα καλο ετοιμο) κλεινω το gmaping στο τερμιναλ που ειναι και τρεχω εκει αυτο
```bash
roslaunch talos_navigation move_base_teb.launch
```
