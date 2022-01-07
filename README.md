# robosis_ros1
ロボットシステム学課題２
# 概要
ROSを使い、プログラムを実行する。
# 環境
・Rasberry Pi 4
      
   ・Ubuntu 20.04 
   
   ・ROS1
# 使用方法
・Ubuntu20.04にros noeticをインストールする（18.04の場合 ros melodic , 16.04の場合 ros kinetic）
    
   ・ホームディレクトリにcatkin_ws/srcを作成
         
      $ cd catkin_ws/src
   
   ・catkin_ws/src内でcatkin_init_workspaceを行う
      
      $ catkin_init_workspace
   
   ・catkin_wsのディレクトリでcatkin_makeからのsource ~/.bashをする
      
      $ cd catkin_ws
      $ catkin_make
      $ source ~/.bash
      
   ・catkin_ws/src内でcatkin_create_pkg mypkg rospyをする
      
      $ cd catkin_ws/src
      $ catkin_create_pkg mypkg rospy
      
   ・パッケージ内にscriptsというディレクトリを作成
   　 
     
      $ cd mypkg/
      $ mkdir scripts
      $ cd scripts/
      
    ・catkin_ws/src/mypkg/scripts内でchmod +x count.pyとchmod +x twice.pyをする
    
    　$ chmod +x count.py
      $ chmod +x twice.py
      
    ・Ubuntuを４つ出し、一つ目はroscore、二つ目は、rosrun mypkg count.py、三つめは、rosrun mypkg twice.py、４つ目はrostopic echo /twiceを実行する
    
      1 $ roscore
      2 $ rosrun mypkg count.py
      3 $ rosrun mypkg twice.py
      4 $ rostopic echo /twice
     すると、２ずつふえる数字が表示される。
     
# ライセンス
