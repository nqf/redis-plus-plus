project(redis++)
cmake_minimum_required(VERSION 3.5)
add_library(redis++ STATIC 
src/sw/redis++/command.cpp         
src/sw/redis++/crc16.cpp         
src/sw/redis++/redis.cpp    
src/sw/redis++/shards_pool.cpp
src/sw/redis++/command_options.cpp  
src/sw/redis++/errors.cpp         
src/sw/redis++/reply.cpp     
src/sw/redis++/subscriber.cpp
src/sw/redis++/connection.cpp       
src/sw/redis++/pipeline.cpp       
src/sw/redis++/sentinel.cpp  
src/sw/redis++/transaction.cpp
src/sw/redis++/connection_pool.cpp  
src/sw/redis++/redis_cluster.cpp 
src/sw/redis++/shards.cpp
)
target_include_directories(redis++ PUBLIC  ${PROJECT_SOURCE_DIR}/sw/redis++/)

