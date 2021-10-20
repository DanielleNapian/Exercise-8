# Lecture/Exercise-8
//SWITCH MONTHS

    #include<stdio.h> 
    void main()
    {
        int a;
        clrscr();
        printf("Enter any Month : ");
        scanf("%d", &a);
        switch (a)
        {
        case 1:
            printf("there are 31 days in Jan ");
            break;
        case 2:
            printf("there are 28 days in Feb");
            break;
        case 3:
            printf("there are 31 days in March");
            break;
        case 4:
            printf("there are 30 days in April");
            break;
        case 5:
            printf(" there are 31 days in May");
            break;
        case 6:
            printf("there are 30 days in June");
            break;
        case 7:
            printf("there are 31 days in July");
            break;
        case 8:
            printf("there are 31 days in August");
            break;
        case 9:
            printf("there are 30 days in Sept.");
            break;
        case 10:
            printf("there are 31 days in Oct.");
            break;
        case 11:
            printf("there are 30 days in Nove.");
            break;
        case 12:
            printf("there are 31 days in Dece.");
            break;
        default:
            printf("it is not found ");
        }
        getch();
    }
//SWITCH GAMEPLAY

    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
        cout << "Would you like to continue playing?\n";
        cout << "Type Y or N\n";

        char input;
        cin >> input;
        switch (input) {
        case 'Y':
        case 'y':
            cout << "Continue playing. . . \n";
            break;
        case 'N':
        case 'n':
            cout << "No I Quit playing. . . \n";
            break;
        default:
            cout << "Invalid Input\n";
        }
    }
//SWITCH FUEL

    #include <iostream>

    using namespace std;
    void fuelex() {
        cout << "Please enter the type of fuel you want to buy (p for petrol, d for diesel) and the amount of litres you need" << endl;
        int litre;
        char fuel;
        double price;
        cout << "Enter the fuel (p or d)" << endl;
        cin >> fuel;
        cout << "Enter the amount of litres needed" << endl;
        cin >> litre;
        if (fuel == 'd' || fuel == 'D') {
            price = litre * 2.51;
            cout << "The price for your fuel is: " << price << endl;
        }
        else {
            switch (fuel) {
            case 'P':
            case 'p':
                price = litre * 2.49;
                cout << "The price for your fuel is: " << price << endl;
                break;
            default:
                cout << "Invalid input" << endl;
            }
        }
        return;
    }
    int main() {
        cout << "Please enter the type of fuel you want to buy (p for petrol, d for diesel) and the amount of litres you need" << endl;
        int litre;
        char fuel;
        double price;
        cout << "Enter the fuel (p or d)" << endl;
        cin >> fuel;
        cout << "Enter the amount of litres needed" << endl;
        cin >> litre;
        if (fuel == 'd' || fuel == 'D') {
            if (isdigit(litre)) {
                price = litre * 2.51;
                cout << "The price for your fuel is: " << price << endl;
            }
        }
        else {
            switch (fuel) {
            case 'P':
            case 'p':
                if (isdigit(litre)) {
                    price = litre * 2.49;
                    cout << "The price for your fuel is: " << price << endl;
                    break;
                }
            default:
                cout << "Invalid input" << endl;
            }
        }
    }
//SWITCH TEPERATURE

    #include<iostream>
    using namespace std;
    int main()
    {
        int a;
        cout << "1. For Celsius To Fahrenheit. \n";
        cout << "2. For Fahrenheit To Celsius. \n";
        cout << "3. For Exit\n\n";
        cout << "Enter Your Choice \n ";
        cin >> a;
        switch (a)
        {
            double cel, feh;
        case 1: cout << "Enter The Temperature In Celsius\n";
            cin >> cel;
            feh = (cel * 9 / 5) + 32;
            cout << "\nTemperature In Fahrenheit Is = " << feh;
            break;

        case 2: cout << "Enter The Temperature In Fahrenheit\n";
            cin >> feh;
            cel = (feh - 32) * 5 / 9;
            cout << "\nTemperature In Celsius Is = " << cel;
            break;

        case 3:exit(0);

        default:cout << "\nEnter The Right Choice \n";
            break;
        }
    }
 //SWITCH NAME OF SHAPES
 
     #include<iostream>
    using namespace std;
    int main()
    {
        int side;
        cout << "Enter the sides number to see the shape name (minimum 3 sides, maximum 10) \n";
        cin >> side;
        switch (side)
        {

        case 1:
        case 2:
        { cout << "The minimum side required is 3, you have entered less than the requirement" << endl; break; }
        case 3:
        { cout << "Triangle  has " << side << " sides" << endl;
        break;
        }
        case 4:
        { cout << "Square | Rectangle has " << side << " sides" << endl;
        break;
        }
        case 5:
        {cout << "Pentagon has " << side << " sides" << endl;
        break;
        }
        case 6:
        { cout << "Hexagon has " << side << " sides" << endl;
        break;
        }
        case 7:
        { cout << "Heptagon has " << side << " sides" << endl;
        break;
        }
        case 8:
        { cout << "Octagon has " << side << " sides" << endl;
        break;
        }
        case 9:
        { cout << "Nonagon has " << side << " sides" << endl;
        break;
        }
        case 10:
        { cout << "Decagon has " << side << " sides" << endl;
        break;
        }
        default:
        {
            cout << "Incorrect command" << endl;
            break;
        }

        }


    }
  //SWITCH CAPITAL OF FRANCE
  
      #include <iostream>
    using namespace std;
    int main()
    {
        cout << "What is the capital of France? Select the option from below\n";
        cout << "\n Enter 'P' for Paris";
        cout << "\n Enter 'D' for Dubai";
        cout << "\n Enter 'N' if you don't know\n";
        char capital;
        cin >> capital;
        switch (capital)
        {
        case 'P':
        case 'p':
        {
            cout << "You're right, the capital of France is Paris" << endl;
            break;
        }
        case 'd':
        case 'D':
        {
            cout << "You're wrong, the capital of France is Paris not Dubai " << endl;
            break;
        }
        case 'n':
        case 'N':
        {
            cout << "The capital of France is Paris" << endl;
            break;
        }
        default:
        {
            cout << "Incorrect command";

        }
        }

        return 0;
    }
//SWITCH GRADE
    
    #include <iostream>
    #include <exception>
    #include <string>

    using namespace std;
    int main()
    {




        cout << "Enter your full name" << endl;
        string name;
        // cin cannot read spaces, that is why we can use the getline code to read the input untill the next line
        getline(cin, name);


        cout << "\nEnter The Marks Between 0 To 100 to check your grade:";

        cout << "\nEnter The Mark: ";
        int marks;

        std::cin >> marks;
        //Using the cin.fail function (when user enters alphabet instead of numbers)
        if (std::cin.fail())
        {
            std::cin.clear();
            std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
            std::cout << "Incorrect command\n: ";
        }

        else if (marks > 100)

        {

            /* Marks greater than 100 */

            cout << "\nKindly input your Marks Between Limit\n";
        }

        else

        {

            switch (marks / 10)

            {

            case 10:

            case 9:
            case 8:

            {
                /* Marks between 80-100 */


                cout << name << " Your Grade Is: A Excellent";


                break;
            }
            case 7:

            {    /* Marks between 70-79 */


                cout << name << " Your Grade Is: B Very Good";


                break;
            }
            case 6:
            {
                /* Marks between 60-69 */


                cout << name << " Your Grade Is: C Fair";

                break;
            }
            case 5:
            {
                /* Marks between 50-59 */

                cout << name << " Your Grade Is: D Need more practice";


                break;
            }
            case 4:
            {
                /* Marks between 40-49 */



                cout << name << " Your Grade Is: E Need more practice";



                break;
            }
            default:
            {
                /* Marks less than 40 */


                cout << name << " You Grade Is: F or Fail\n";


            }
            }
        }
    }
