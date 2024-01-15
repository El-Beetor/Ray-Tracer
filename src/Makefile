CC = g++
CFLAGS = -Wall -std=c++17

TARGET = my_program
SOURCES = main.cpp 
OBJECTS = $(SOURCES:.cpp=.o)

# Add the header file to the dependencies
DEPS = vec3.h color.h

$(TARGET): $(OBJECTS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJECTS)

%.o: %.cpp $(DEPS)
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(TARGET) $(OBJECTS)
