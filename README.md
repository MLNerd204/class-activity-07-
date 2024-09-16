#include <iostream>
#include <string>

int main() {
    // Define an array to hold three names
    const int numNames = 3;
    std::string names[numNames];
      // Prompt the user to enter three names
    std::cout << "Please enter three names:\n";
    for (int i = 0; i < numNames; ++i) {
        std::cout << "Name " << (i + 1) << ": ";
        std::getline(std::cin, names[i]);
    }

      // Print the first name
    std::cout << "\nThe first name you entered is: " << names[0] << std::endl;

    return 0;
}


in this code const int numNames = 3;: Constant for the number of names.
std::string names[numNames];: Array to store the names.

The for loop iterates three times, asking the user for each name and storing it in the names array.
std::getline(std::cin, names[i]); is used to read the entire line including spaces.

After all names are entered, the program prints the first name stored in the array.
