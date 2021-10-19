# Lecture7HW
Lecture 7 Homework : Compound Conditions and Nested Statments

# MARK MY WORDS ppt.16

        #include <iostream>
        using namespace std;

        int main()
        {
         int testScore;
            cout << "Insert score to determine the grade: \n";
             cin >> testScore;


    if (testScore >= 70 && testScore <= 100) {
        cout << "A! Outstanding!";

    }else if (testScore >= 60 && testScore <= 69) {
        cout << "B! Great!";

    }else if (testScore >= 50 && testScore <= 59) {
        cout << "C! Adequate!";
    }
    else if (testScore >= 40 && testScore <= 49) {
        cout << "D! Almost!";
    }
    else if (testScore >= 40) {
        cout << "F! Study! Never Give Up!";
    }

    return 0;

    }
  
  # STARING A BAND ppt.17

        #include <iostream>
        #include <string>
        using namespace std;

    int main()
    {
    bool musicFriend = true;
    string friendPlaysgui = "guitar";
    string friendPlaysdru = "drums";

    cout << "Can you start a band with this person ? \n";
    
    if (musicFriend) {
        if (friendPlaysgui == "guitar") {
            cout << "You can start a band!";
        }
        else if (friendPlaysdru == "drums") {
            cout << "You can start a band!";
        }
        else {
            cout << "Gotta find new members bro!";
        }
    }

    }


  # Killing Time ppt.19
      //yay i got it right i think
      //7:38PM NICE I GOT IT
  
    #include <iostream>
    using namespace std;
    int main()
    {
    bool bestie = true;
    bool fiveAed = true;
    int time;

    cout << "You're in Dubai Mall. Your bestie just called, \n";
    cout << "How many minutes did they say they'll be arriving? \n";

    cin >> time;

    if (bestie) {
        if (time >= 15) {
            if (fiveAed) {
                cout << "This might take a while, go buy a cofee worth 5 AED. Go window shopping while you're at it";
            }
        }
        else if (time <= 14) {
            cout << "Wait in the food court. Play games on your phone while you're waiting.";
        }
        else {
            cout << "They stood you up. Go back home. #fakefriend";
        }
    }
}



# Earthquake ppt.20
                    
    //practice makes perfect even with 4gb ram

    #include <iostream>
    using namespace std;

    int main() {

    double magn;
    bool earthquake = true;

    cout << "The ground is shaking! What does the Richter scale says about its power level?\n";
    cin >> magn;

    if (earthquake) {
        if (magn <= 2.0) {
            cout << "It's a Micro level earthquake.";
        }
        else if (magn <= 3.0) {
            cout << "Very minor earthquake. Exercise minimal caution.";
        }
        else if (magn <= 4.0) {
            cout << "Minor earthquake. Careful.";
        }
        else if (magn <= 5.0) {
            cout << "Light earthquke. Take safety measurements.";
        }
        else if (magn <= 6.0) {
            cout << "Moderate earthquake. Brace for ground shakes.";
        }
        else if (magn <= 7.0) {
            cout << "Strong earthquke. Move to a safeguarded vicinity.";
        }
        else if (magn <= 8.0) {
            cout << "Major earthquake. Transfer to a designated earthquake-proof area.";
        }
        else if (magn <= 9.0) {
            cout << "Great earthquake. Please leave your houses and relocate at earthquake-proof buildings for safety.";
        }
        else if (magn >= 10.0) {
            cout << "WARNING : METEORIC EARTHQUAKE | PLEASE REMAIN CALM\n";
            cout << "THIS IS NOT A DRILL | SEEK IMMEDIATE SHELTER\n";
            cout << "PROCEED TO NEAR ANTI EARTHQUAKE BUIDINGS";
        }
    }
    else {
        cout << "No earthquake detected, carry on.";
    }
    return 0;
    }

# Lecture 8
Switch Statements 

# Fuel
        #include <iostream>
        using namespace std;
        int main()
        {

    char gas;
    int gasAmt;

    cout << "Welcome to the automatic gas service! Please enter your type of fuel to continue \n";
    cout << "[P] for Petrol or [D] for Diesel \n";
    cin >> gas;


    switch (gas)
    {
    case 'p':
    case 'P':
        cout << "You chose petrol, how many liters do you need? Rate: 2AED Per liter\n";
        cin >> gasAmt;
        cout << "You entered " << gasAmt << " liters. That would be " << gasAmt * 2 << " AED";

        break;
    
    case 'd':
    case 'D':
        cout << "You chose diesel, how many liters do you need? Rate: 3AED Per liter\n";
        cin >> gasAmt;
        cout << "You entered " << gasAmt << " liters. That would be " << gasAmt * 3 << " AED";

        break;
    default:
        cout << "Invalid input";

        return 0;

    }
    }


# Temperature
        #include <iostream>
        using namespace std;
        int main()
        {

    char temp;
    double tempInput;

    cout << "Converting temperatures! Would you like convert Celsius to Farenheit? or Farenheit to Celsius? \n";
    cout << "[C] for C to F or [F] for F to C \n";
    cin >> temp;


    switch (temp)
    {
    case 'C':
    case 'c':
        cout << "Insert temperature in Celsius to convert in Farenheit\n";
        cin >> tempInput;
        cout << "You entered " << tempInput << "C's. That would be " << (tempInput * 1.8) + 32 << " Degrees Farenheit";

        break;

    case 'F':
    case 'f':
        cout << "Insert temperature in Farenheit to convert in Celsius\n";
        cin >> tempInput;
        cout << "You entered " << tempInput << ". That would be " << 5 * (tempInput - 32) / 9 << " Degrees Celcius";

        break;
    default:
        cout << "Invalid input! Please enter a number.";

        return 0;

    }
    }

 # Capital of France
        #include <iostream>
        using namespace std;
        int main()
        {
    cout << "What is the capital of France?\n";
    cout << "Press [P] for Paris\n";
    cout << "Press [D] for Dubai\n";
    cout << "Press [A] for Alabama\n";
    cout << "Press [W] for Washington \n";

    char capital;
    cin >> capital;

    switch (capital)
    {
    case 'P':
        cout << "Correct! \n";
        break;
    case 'p':
        cout << "Correct! \n";
        break;

    case 'D':
        cout << "Incorrect \n";
        break;
    case 'd':
        cout << "Incorrect \n";
        break;
    case 'A':
        cout << "Incorrect \n";
        break;
    case 'a':
        cout << "Incorrect \n";
        break;
    case 'W':
        cout << "Incorrect \n";
        break;
    case 'w':
        cout << "Incorrect \n";
        break;
    
         
    default:
        cout << "Invalid \n";
        break;
    } 
    }

# Shapes Switch 
        #include <iostream>
        using namespace std;
        int main()
        {
    int number;
    cout << "Give a number to determine its shape \n";
    cin >> number;

    switch (number)
    {
    case 3:
        cout << "Triangle";
        break;
    case 4:
        cout << "Square/Rectangle";
        break;
    case 5:
        cout << "Pentagon";
        break;
    case 6:
        cout << "Hexagon";
        break;
    case 7:
        cout << "Heptagon";
        break;
    case 8:
        cout << "Octagon";
        break;
    case 9:
        cout << "Nonagon";
        break;
    case 10:
        cout << "Decagon";
        break;
    default:
        cout << "Invalid \n";
        break;
    }

    }
    
    
# Grades
        #include <iostream>
        #include <string>
        using namespace std;
        int main()
        {
    string name;
    string lastname;
    int grade;

    cout << "Enter student's first name \n";
    cin >> name;
    cout << "Enter student's last name: \n";
    cin >> lastname;
    cout << "Enter the grade of " << name << " " << lastname << " to determine its mark. \n";
    cout << "Enter [1] If score is more than 70% \n";
    cout << "Enter [2] If score is 69-60% \n";
    cout << "Enter [3] If score is 59-50% \n";
    cout << "Enter [4] If score is 49-40% \n";
    cout << "Enter [5] If score is less than 39% \n";
    cin >> grade;
    
    switch (grade)
    {
    case 1:
        cout << name << " " << lastname << ", A";
        break;
    case 2:
        cout << name << " " << lastname << ", B";
        break;
    case 3:
        cout << name << " " << lastname << ", C";
        break;
    case 4:
        cout << name << " " << lastname << ", D";
        break;
    case 5:
        cout << name << " " << lastname << ", F";
        break;
    default:
        cout << "Invalid input. \n";
    }
        }

# Grades 2.0 (User can input full name)
        #include <iostream>
        #include <string>
        using namespace std;
        int main()
        {
    string name;
    int grade;

    cout << "Enter student's full name: \n";
    getline(cin, name);
    cout << "Enter the grade of " << name << " to determine its mark. \n";
    cout << "Enter [1] If score is more than 70% \n";
    cout << "Enter [2] If score is 69-60% \n";
    cout << "Enter [3] If score is 59-50% \n";
    cout << "Enter [4] If score is 49-40% \n";
    cout << "Enter [5] If score is less than 39% \n";
    cin >> grade;

    switch (grade)
    {
    case 1:
        cout << name << "- A";
        break;
    case 2:
        cout << name <<  "- B";
        break;
    case 3:
        cout << name <<  "- C";
        break;
    case 4:
        cout << name <<  "- D";
        break;
    case 5:
        cout << name << "- F";
        break;
    default:
        cout << "Invalid input. \n";
    }

        }
