#include<iostream> 
using namespace std;

void MonsterGen();

int main() {
	char input;  
		while (1) {
		MonsterGen();
		cout << "press any key to continue..." << endl;
		cin >> input;
	}

}
void MonsterGen() {
	int num = rand() % 100 + 1;
	if (num < 15)
		cout << "A Wraith Spawned." << endl;
	else if (num < 20)
		cout << "A Demon Spawned." << endl;
	else if (num < 50)
		cout << "An Phantom Spawned." << endl;
	else if (num < 75)
		cout << "A Spirit Spawned." << endl;
	else if (num < 100)
		cout << "An Revenant Spawned." << endl;
}
