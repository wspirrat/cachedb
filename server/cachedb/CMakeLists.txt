# Copyright (c) Meta Platforms, Inc. and affiliates.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

cmake_minimum_required (VERSION 3.12)

project (cachelib-cmake-test-project VERSION 0.1)

find_package(cachelib CONFIG REQUIRED)

# set(cachelib_DIR "../.." CACHE PATH "cachelib/cmake")

add_executable(cachedb cache.cpp)

target_link_libraries(cachedb cachelib)
