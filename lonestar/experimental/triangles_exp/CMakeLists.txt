find_package(Eigen)
if(Eigen_FOUND)
  include_directories(${Eigen_INCLUDE_DIRS})
  add_definitions(-DHAS_EIGEN)
endif()
app(triangles-exp Triangles.cpp)
