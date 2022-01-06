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
      
   
   ・
