cmake_minimum_required(VERSION 2.8.3)
project(s_rov_messages)

find_package(catkin REQUIRED COMPONENTS
  message_generation
)

add_message_files(
  DIRECTORY msg
  FILES
  pwm.msg
)

generate_messages()

catkin_package(
  CATKIN_DEPENDS message_runtime
)
