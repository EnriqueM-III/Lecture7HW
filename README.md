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
