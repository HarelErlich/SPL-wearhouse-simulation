
CXX = g++
CXXFLAGS = -g -Wall -Weffc++

SRC_DIR = src
BIN_DIR = bin

EXEC_NAME = warehouse

all: clean compile link 

link:
	$(CXX) -o $(BIN_DIR)/$(EXEC_NAME) $(BIN_DIR)/main.o $(BIN_DIR)/WareHouse.o $(BIN_DIR)/Customer.o $(BIN_DIR)/Order.o $(BIN_DIR)/Action.o $(BIN_DIR)/Volunteer.o

compile:
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/main.o $(SRC_DIR)/main.cpp
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/WareHouse.o $(SRC_DIR)/WareHouse.cpp
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/Customer.o $(SRC_DIR)/Customer.cpp
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/Volunteer.o $(SRC_DIR)/Volunteer.cpp
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/Order.o $(SRC_DIR)/Order.cpp
	$(CXX) $(CXXFLAGS) -c -o $(BIN_DIR)/Action.o $(SRC_DIR)/Action.cpp

clean:
	rm -f $(BIN_DIR)/*

.PHONY: all clean compile link 