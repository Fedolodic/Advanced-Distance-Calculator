//  Advanced Distance Calculator
//
//  Created by David Martinez on 1/28/16.
//  Copyright © 2016 Joenteny David Martinez Gutierrez. All rights reserved.
//
//  Description:
//  Calculates mph, kph and nlypm (nanolightyears per minute) based on miles and time, in hours, input

#include <iostream>
#include <string>
#include <iomanip>
#include <cmath>

using namespace std;

double calculatemph(double, double);    // calculatemph function prototype

int main()
{
    double miles;           // miles is a type of double
    double hours;           // hours is a type of double
    double mph;             // mph is a type of double
    double kph;             // kph is a type of double
    double nlypm;           // nlypm is a type of double
    string milesCorrect;    // milesCorrect is a type of string
    string hoursCorrect;    // hoursCorrect is a type of string
    
    
    // Get miles from user
    cout << "Please enter distance traveled in miles: ";
    cin >> miles;
    
    // Input validation for miles
    while (miles < 1)
    {
        cout << "Error! That value won't work! Value must be a positive non-zero number." << endl;
        
        cout << "Please enter distance traveled in miles: ";
        cin >> miles;
    }
    
    // Ask user to verify input was correct
    cout << "You entered " << miles << " miles is this correct?" << endl;
    cout << "Please enter 'Yes' or 'No': ";
    cin >> milesCorrect;
    
    // while loop if user input was incorrect
    while (milesCorrect == "No" || milesCorrect == "no")
    {
        cout << "Please enter distance traveled in miles: ";
        cin >> miles;
        
        while (miles < 1)
        {
            cout << "Error! That value won't work! Value must be a positive non-zero number." <<endl;
            
            cout << "Please enter distance traveled in miles: ";
            cin >> miles;
        }
        
        cout << "You entered " << miles << " miles is this correct?" << endl;
        cout << "Please enter 'Yes' or 'No': ";
        cin >> milesCorrect;
    }
    
    // Get hours from user
    cout << "Please enter time taken in hours: ";
    cin >> hours;
    
    // Input validation for hours
    while (hours < 1)
    {
        cout << "Error! That value won't work! Value must be a positive non-zero number." << endl;
        
        cout << "Please enter time taken in hours: ";
        cin >> hours;
    }
    
    // Ask user to verify is input was correct
    cout << "You entered " << hours << " hours is this correct?" << endl;
    cout << "Please enter 'Yes' or 'No': ";
    cin >> hoursCorrect;
    
    // while loop if user input was incorrect
    while (hoursCorrect == "no" || hoursCorrect == "No")
    {
        cout << "Please enter time taken in hours: ";
        cin >> hours;
        
        while (hours < 1)
        {
            cout << "Error! That value won't work! Value must be a positive non-zero number." << endl;
            
            cout << "Please enter time taken in hours: ";
            cin >> hours;
        }
        
        cout << "You entered " << hours << " hours is this correct?" << endl;
        cout << "Please enter 'Yes' or 'No': ";
        cin >> hoursCorrect;
    }
    
    // Calculate mph, kph and nlypm
    mph = calculatemph(miles, hours);
    kph = mph * 1.60934;
    nlypm = kph * 1.762 * pow(10, -6);
    
    // Display mph, kph and nlypm
    cout << fixed << setprecision(2) << "Your miles per hour is " << mph << " mph" << endl;
    cout << fixed << setprecision(2) << "Your kilometers per hour is " << kph << " kph" << endl;
    cout << fixed << setprecision(8) << "Your nanolightyears per minute is " << nlypm << " nlypm" << endl;
    
    return 0;
}   // End of function main ()

double calculatemph(double miles, double hours)
{
    double mph; // mph is a type of double
    
    // Calculate mph
    mph = miles/hours;
    
    // Return mph
    return mph;
}   // End of function calculatemph ()
