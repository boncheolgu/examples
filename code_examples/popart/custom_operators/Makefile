CXX ?= g++
CXXFLAGS = -std=c++11 -ggdb3 -O3
LDLIBS = -lpopart -lpoplar -lpopops

BUILD_DIR = build
SOURCES = cube_fn_custom_op.cpp
TARGET = $(BUILD_DIR)/cube_fn_custom_op

all: create_build_dir cube_fn_custom_op 

.PHONY: create_build_dir
create_build_dir: 
	mkdir -p $(BUILD_DIR)

cube_fn_custom_op: cube_fn_custom_op.cpp
	$(CXX) $(SOURCES)  $(LDLIBS) $(CXXFLAGS) -o $(TARGET)

.PHONY: clean
clean:
	rm -r  $(BUILD_DIR)
