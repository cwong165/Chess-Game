Project(Chess)
CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

SET(CMAKE_CXX_STANDARD 11)

ADD_SUBDIRECTORY(googletest)

ADD_EXECUTABLE(test
    player_test.cpp
    board.cpp
    Game.cpp    
)

ADD_EXECUTABLE(CHESS
    main.cpp
    board.cpp
    Game.cpp    
)
TARGET_LINK_LIBRARIES(test gtest)
TARGET_COMPILE_DEFINITIONS(test PRIVATE gtest_disable_pthreads=ON)

