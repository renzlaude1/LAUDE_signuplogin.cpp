# LAUDE_signuplogin.cpp

// sign_in.cpp
#include <iostream>
#include <string>

int main() {
    // Hardcoded credentials
    const std::string correctUsername = "admin";
    const std::string correctPassword = "12345";

    std::string inputUsername, inputPassword;

    std::cout << "=== Sign In ===\n";
    std::cout << "Username: ";
    std::getline(std::cin, inputUsername);

    std::cout << "Password: ";
    std::getline(std::cin, inputPassword);

    if (inputUsername == correctUsername && inputPassword == correctPassword) {
        std::cout << "Sign in successful! Welcome, " << inputUsername << "!\n";
    } else {
        std::cout << "Sign in failed. Incorrect username or password.\n";
    }

    return 0;
}
