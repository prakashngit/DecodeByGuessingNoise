CXX=g++
CXXFLAGS= -w -Wall -pthread -m64

SINGSRC=simulate.cpp
SOURCES = channel/channelModel.cpp
OBJECTS=$(SOURCES:.cpp=.o) 
HEADERS=$(SOURCES:.cpp=.hpp) 
EXECUTABLE=simulate

all: $(SOURCES) $(HEADERS) $(SINGSRC) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CXX)  $(CXXFLAGS) $(OBJECTS) -o $(EXECUTABLE)

.cpp.o:
	$(CXX) $(CXXFLAGS) -c $< -o $@
	
