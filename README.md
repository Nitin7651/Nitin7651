#include <iostream>
#include <cstdlib>
#include <ctime>

int main()
 {
    srand(time(0));
    int secretnumber= rand() % 100 + 1;

    int guess;
    std::cout << "Guess a Numberumber between 1 to 100: ";
    std::cin >> guess;
    while (guess != secretnumber)
     {
        if (guess < secretnumber)
        {
            std::cout << "Too low!" << std::endl;
        } else
        {
            std::cout << "Too high!" << std::endl;
        }
        std::cout << "Try again: ";
        std::cin >> guess;
    }

    
    std::cout << "Congratulations! You guessed the correct Number." << std::endl;

    return 0;
