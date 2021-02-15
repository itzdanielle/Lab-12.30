# Lab-12.30
#include <iostream>
using namespace std;

int main() {
  double numHours, average;
	int numStudents;
	double total = 0;

	cout << "This program will find the average number of hours"
		<< " that students spent studying for biolody and programming over a weekend" << endl << endl;
	cout << "How many students are there?" << endl;
	cin >> numStudents;

	for (int student = 1; student <= numStudents; student++)
	{
		cout << endl << "Please enter the number of hours worked by student for biology "
			<< student << " over the weekend." << endl;
		cin >> numHours;
    cout << endl << "Please enter the number of hours worked by student for programming "
			<< student << " over the weekend." << endl;
		cin >> numHours;
		total = total + numHours;
	}

	average = total / numStudents;

	cout << endl;
	cout << "The average number of spent programming by "
		<< "the students was " << average << endl << endl << endl;
}
