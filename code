#include <iostream> // input output 
#include <cstdlib>  // random
#include <ctime>    // time
#include <string>   // string
using namespace std;
//list of functions
void fail(const string& prompt, int& value);
void intro();
void OpeningScreen(int& option, string& p1Name, string& p2Name, string& p3Name);

void startcards(int& c1, int& c2, int& c3, int& c4, int& c5, int& c6,
                int& p2c1, int& p2c2, int& p2c3, int& p2c4, int& p2c5, int& p2c6,
                int& p3c1, int& p3c2, int& p3c3, int& p3c4, int& p3c5, int& p3c6);

void ArtsP1(int& card, int& c1, int& c2, int& c3, int& c4, int& c5, int& c6,
            string& c1art, string& c2art, string& c3art, string& c4art, string& c5art, string& c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

void ArtsP2(int& card, int& p2c1, int& p2c2, int& p2c3, int& p2c4, int& p2c5, int& p2c6,
            string& p2c1art, string& p2c2art, string& p2c3art, string& p2c4art, string& p2c5art, string& p2c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

void ArtsP3(int& card, int& p3c1, int& p3c2, int& p3c3, int& p3c4, int& p3c5, int& p3c6,
            string& p3c1art, string& p3c2art, string& p3c3art, string& p3c4art, string& p3c5art, string& p3c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

string getCardName(int card);
int getCardValueForpoints(int card);
string lookupArt(int card,
                 string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
                 string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
                 string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
                 string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

int playTurn(int cards1[6], int cards2[6], int cards3[6], string& p1Name, string& p2Name, string& p3Name,
             int& p1score, int& p2score, int& p3score,
             int& p1round, int& p2round, int& p3round,
             int& leader,
             bool& p2alive, bool& p3alive,
             string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
             string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
             string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
             string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

int playRound(int cards1[6], int cards2[6], int cards3[6], string& p1Name, string& p2Name, string& p3Name,
              int& p1score, int& p2score, int& p3score,
              bool& p2alive, bool& p3alive, int& leader,
              string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
              string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
              string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
              string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK);

void playGame();

bool askPlayAgain();
bool handlePlayerElimination(int& p1score, int& p2score, int& p3score);

int chooseCardForAI(int cards[6], int refCard);

int main() {
	srand(time(0));
	playGame();
	return 0;
}

string getCardName(int card) { //makes card names based off
	static const string ranks[] = {"A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"};
	static const string suits[] = {"Clubs", "Spades", "Diamonds", "Hearts"};
	int idx = card - 1;
	int suit = idx / 13;
	int rank = idx % 13;
	return ranks[rank] + " of " + suits[suit]; //displays card info
}

int getCardValueForpoints(int card) { //depending on the card picked it assigns values
	int r = (card - 1) % 13 + 1;
	return r;
}

string lookupArt(int card, // depending on card value assigns different art
                 string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
                 string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
                 string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
                 string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {
	if(card==1) return ClA;
	else if(card==2) return Cl2;
	else if(card==3) return Cl3;
	else if(card==4) return Cl4;
	else if(card==5) return Cl5;
	else if(card==6) return Cl6;
	else if(card==7) return Cl7;
	else if(card==8) return Cl8;
	else if(card==9) return Cl9;
	else if(card==10) return Cl10;
	else if(card==11) return ClJ;
	else if(card==12) return ClQ;
	else if(card==13) return ClK;
	else if(card==14) return SA;
	else if(card==15) return S2;
	else if(card==16) return S3;
	else if(card==17) return S4;
	else if(card==18) return S5;
	else if(card==19) return S6;
	else if(card==20) return S7;
	else if(card==21) return S8;
	else if(card==22) return S9;
	else if(card==23) return S10;
	else if(card==24) return SJ;
	else if(card==25) return SQ;
	else if(card==26) return SK;
	else if(card==27) return DA;
	else if(card==28) return D2;
	else if(card==29) return D3;
	else if(card==30) return D4;
	else if(card==31) return D5;
	else if(card==32) return D6;
	else if(card==33) return D7;
	else if(card==34) return D8;
	else if(card==35) return D9;
	else if(card==36) return D10;
	else if(card==37) return DJ;
	else if(card==38) return DQ;
	else if(card==39) return DK;
	else if(card==40) return HA;
	else if(card==41) return H2;
	else if(card==42) return H3;
	else if(card==43) return H4;
	else if(card==44) return H5;
	else if(card==45) return H6;
	else if(card==46) return H7;
	else if(card==47) return H8;
	else if(card==48) return H9;
	else if(card==49) return H10;
	else if(card==50) return HJ;
	else if(card==51) return HQ;
	else if(card==52) return HK;
	return "";
}

bool askPlayAgain() { //asks if player would like to play again and takes in input
	int choice;
	while (true) {
		cout << "\nPlay again?\n1. Yes\n 2. No\nInput: ";
		cin >> choice;

		if (cin.fail()) {
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid input. Try again.\n";
		} else if (choice == 1) {
			return true;
		} else if (choice == 2) {
			return false;
		} else {
			cout << "Please enter 1 or 2.\n";
		}
	}
}

bool handlePlayerElimination(int& p1score, int& p2score, int& p3score) { //depending on player score itll kick out the player
	if (p1score <= 0) {
		cout << "You lost\n";
		return true;
	}
	return false;
}

void playGame() { //variables for playing game
	int option;
	string p1Name;
	string p2Name;
	string p3Name;

	string c1art, c2art, c3art, c4art, c5art, c6art;
	string p2c1art, p2c2art, p2c3art, p2c4art, p2c5art, p2c6art;
	string p3c1art, p3c2art, p3c3art, p3c4art, p3c5art, p3c6art;
	string ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK;
	string SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK;
	string DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK;
	string HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK;

	int c1, c2, c3, c4, c5, c6;
	int p2c1, p2c2, p2c3, p2c4, p2c5, p2c6;
	int p3c1, p3c2, p3c3, p3c4, p3c5, p3c6;

	intro();

	bool playAgain = true;
	int leader = 1;

	while (playAgain) {
		OpeningScreen(option, p1Name, p2Name, p3Name); //scores display

		int p1score = 30;
		int p2score = 30;
		int p3score = 30;

		bool p2alive = true;
		bool p3alive = true;

		int again = 1;
		do {
			if (p1score <= 0 || (!p2alive && !p3alive)) {
				break;
			}

			startcards(c1, c2, c3, c4, c5, c6,
			           p2c1, p2c2, p2c3, p2c4, p2c5, p2c6,
			           p3c1, p3c2, p3c3, p3c4, p3c5, p3c6);

			int cards1[6] = {c1, c2, c3, c4, c5, c6};
			int cards2[6] = {p2c1, p2c2, p2c3, p2c4, p2c5, p2c6};
			int cards3[6] = {p3c1, p3c2, p3c3, p3c4, p3c5, p3c6};

			cout << "\nYour cards:\n";
			for (int i = 0; i < 6; i++) {
				cout << (i + 1) << ") " << getCardName(cards1[i]) << "\n";
			}
			cout << "\n";

			ArtsP1(c1, c1, c2, c3, c4, c5, c6, //variables for card art
			       c1art, c2art, c3art, c4art, c5art, c6art,
			       ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			       SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			       DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			       HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);

			leader = playRound(cards1, cards2, cards3, p1Name, p2Name, p3Name, //varibales for art in rounds
			                   p1score, p2score, p3score,
			                   p2alive, p3alive, leader,
			                   ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                   SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                   DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                   HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);

			if (p2score <= 0 && p2alive) {
				p2alive = false;
				cout << p2Name << " has been eliminated!\n";
			}

			if (p3score <= 0 && p3alive) {
				p3alive = false;
				cout << p3Name << " has been eliminated!\n";
			}

			if (p1score <= 0 || (!p2alive && !p3alive)) {
				break;
			}

			fail("\n1. Begin next round\n2. End game\nInput: ", again);

		} while (again == 1);

		cout << "Game over\n";

		bool endGame = handlePlayerElimination(p1score, p2score, p3score); //checks if game ended

		if (endGame) {
			playAgain = askPlayAgain();
		} else {
			if (p1score > 0 && (!p2alive || !p3alive)) {
				cout << "You defeated all opponents!\n";
			} else {
				cout << "Ended by user.\n";
			}
			playAgain = false;
		}
	}

	cout << "Thanks for playing!\n";
}

int playRound(int cards1[6], int cards2[6], int cards3[6], string& p1Name, string& p2Name, string& p3Name,
              int& p1score, int& p2score, int& p3score,
              bool& p2alive, bool& p3alive, int& leader,
              string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
              string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
              string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
              string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {

	int p1round = 0;
	int p2round = 0;
	int p3round = 0;

	for (int t = 0; t < 6; t++) {
		if (p1score <= 0 || (p2score <= 0 && p3score <= 0)) {
			break;
		}

		leader = playTurn(cards1, cards2, cards3, p1Name, p2Name, p3Name,
		                  p1score, p2score, p3score,
		                  p1round, p2round, p3round,
		                  leader,
		                  p2alive, p3alive,
		                  ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
		                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
		                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
		                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);

		if (p1score <= 0 || (p2score <= 0 && p3score <= 0)) {
			break;
		}

		int remaining = 0;
		cout << "\nCards remaining in your hand:\n";
		for (int i = 0; i < 6; i++) {
			if (cards1[i] != 0) {
				remaining++;
				cout << (i + 1) << ") " << getCardName(cards1[i]) << "\n";
			}
		}
		cout << "Total remaining: " << remaining << "\n\n";
	}
	return leader;
}

int chooseCardForAI(int cards[6], int refCard) {
	if (cards == nullptr) return -1;
	int index = -1;
	if (refCard != -1) {
		for (int i = 0; i < 6 && index == -1; i++) {
			if (cards[i] != 0 && cards[i] > refCard) index = i;
		}
	}
	if (index == -1) {
		int low = 100;
		for (int i = 0; i < 6; i++) {
			if (cards[i] != 0 && cards[i] < low) {
				low = cards[i];
				index = i;
			}
		}
	}
	if (index == -1) return 0;
	return index;
}

int playTurn(int cards1[6], int cards2[6], int cards3[6], string& p1Name, string& p2Name, string& p3Name,
             int& p1score, int& p2score, int& p3score,
             int& p1round, int& p2round, int& p3round,
             int& leader,
             bool& p2alive, bool& p3alive,
             string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
             string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
             string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
             string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {

	int p1card = 0, p2card = 0, p3card = 0;
	int refCard = -1;
	auto pause = []() {
		cout << "\nPress ENTER to continue...";
		cin.ignore();
		cin.get();
	};

	auto humanPlay = [&](int cards[6]) {
		int play1;
		int valid = 0;
		do {
			cout << "Choose a card (1-6): ";
			cin >> play1;
			if (!cin.fail() && play1 >= 1 && play1 <= 6 && cards[play1 - 1] != 0) {
				valid = 1;
			} else {
				cin.clear();
				cin.ignore(1000, '\n');
				cout << "Invalid choice. Try again.\n";
			}
		} while (valid == 0);
		int c = cards[play1 - 1];
		cards[play1 - 1] = 0;
		return c;
	};

	auto aiPlay = [&](int cards[6]) {
		int idx = chooseCardForAI(cards, refCard);
		int c = cards[idx];
		cards[idx] = 0;
		return c;
	};

	if (leader == 1) {
		// Player 1
		p1card = humanPlay(cards1);
		refCard = p1card;
		cout << p1Name << " played: " << getCardName(p1card) << "\n";
		cout << lookupArt(p1card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
		                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
		                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
		                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
		pause();

		if (p2alive) {
			p2card = aiPlay(cards2);
			cout << p2Name << " played: " << getCardName(p2card) << "\n";
			cout << lookupArt(p2card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}

		if (p3alive) {
			p3card = aiPlay(cards3);
			cout << p3Name << " played: " << getCardName(p3card) << "\n";
			cout << lookupArt(p3card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}

	} else if (leader == 2) {

		if (p2alive) {
			p2card = aiPlay(cards2);
			refCard = p2card;
			cout << p2Name << " played: " << getCardName(p2card) << "\n";
			cout << lookupArt(p2card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}

		if (p3alive) {
			p3card = aiPlay(cards3);
			cout << p3Name << " played: " << getCardName(p3card) << "\n";
			cout << lookupArt(p3card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}

		cout << "\nYour turn\n";
		cout << "You must beat: " << getCardName(refCard) << "\n\n";

		p1card = humanPlay(cards1);
		cout << p1Name << " played: " << getCardName(p1card) << "\n";
		cout << lookupArt(p1card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
		                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
		                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
		                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
		pause();

	} else if (leader == 3) {

		if (p3alive) {
			p3card = aiPlay(cards3);
			refCard = p3card;
			cout << p3Name << " played: " << getCardName(p3card) << "\n";
			cout << lookupArt(p3card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}

		cout << "\nYour turn\n";
		cout << "You must beat: " << getCardName(refCard) << "\n\n";

		p1card = humanPlay(cards1);
		cout << p1Name << " played: " << getCardName(p1card) << "\n";
		cout << lookupArt(p1card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
		                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
		                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
		                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
		pause();

		if (p2alive) {
			p2card = aiPlay(cards2);
			cout << p2Name << " played: " << getCardName(p2card) << "\n";
			cout << lookupArt(p2card, ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
			                  SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
			                  DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
			                  HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
			pause();
		}
	}

	int roundCards[3];
	int ids[3];
	int n = 0;

	if (p1card != 0) {
		roundCards[n] = getCardValueForpoints(p1card);
		ids[n++] = 1;
	}

	if (p2alive && p2card != 0) {
		roundCards[n] = getCardValueForpoints(p2card);
		ids[n++] = 2;
	}

	if (p3alive && p3card != 0) {
		roundCards[n] = getCardValueForpoints(p3card);
		ids[n++] = 3;
	}

	if (n == 0) return leader;
	if (n == 1) return ids[0];

	int high   = roundCards[0];
	int low    = roundCards[0];
	int highId = ids[0];
	int lowId  = ids[0];

	for (int i = 1; i < n; i++) {
		if (roundCards[i] > high) {
			high = roundCards[i];
			highId = ids[i];
		}
		if (roundCards[i] < low) {
			low = roundCards[i];
			lowId = ids[i];
		}
	}

	if (highId == 1) p1round++;
	else if (highId == 2) p2round++;
	else p3round++;

	if (lowId == 1) {
		p1round--;
		int v = getCardValueForpoints(p1card);
		p1score -= v;
		cout << "" << p1Name << " loses this turn, -" << v << " points.\n";
	} else if (lowId == 2) {
		p2round--;
		int v = getCardValueForpoints(p2card);
		p2score -= v;
		cout << "" << p2Name << " loses this turn, -" << v << " points.\n";
	} else {
		p3round--;
		int v = getCardValueForpoints(p3card);
		p3score -= v;
		cout << "" << p3Name << " loses this turn, -" << v << " points.\n";
	}

	cout << "\n------------------------\n";  //Winner disp
	if (highId == 1) {
		cout << p1Name << " wins the round!\n";
	} else if (highId == 2) {
		cout << p2Name << " wins the round!\n";
	} else {
		cout << p3Name << " wins the round!\n";
	}
	cout << "------------------------\n";

	cout << "\nScores now:\n"; //Score disp
	cout << "" << p1Name << ": " << p1score << "\n";
	cout << "" << p2Name << ": " << p2score << "\n";
	cout << "" << p3Name << ": " << p3score << "\n";

	return highId;
}

void fail(const string& prompt, int& value) {
	while (true) {
		cout << prompt;
		cin >> value;
		if (cin.fail()) {
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid input. Try again.\n";
		} else {
			break;
		}
	}
}

void intro() {
	cout << "--------------------\n";
	cout << "    G  U  R  K  A   \n";
	cout << "--------------------\n";
}

void OpeningScreen(int& option, string& p1Name, string& p2Name, string& p3Name) {
	do {
		fail("\n1. Start Game\n2. Rules\n\nInput: ", option);
		if (option == 1) {
			cout << "\nWhat is your username?\nInput: ";
			cin >> p1Name;
			cout << "\nWhat is Player 2 (Bot)'s username?\nInput: ";
			cin >> p2Name;
			cout << "\nWhat is Player 3 (Bot)'s username?\nInput: ";
			cin >> p3Name;
			cout << "\nStarting game... \n";
			break;
		}
		else if (option == 2) {
			cout << "\n|-------------------------|\n";
			cout << "|        GURKA RULES      |\n";
			cout << "|-------------------------|\n";
			cout << "| Players: 3              |\n";
			cout << "| Deck: 52 cards          |\n";
			cout << "|-------------------------|\n";
			cout << "| Setup:                  |\n";
			cout << "| - Deal 6 cards per      |\n";
			cout << "|   player                |\n";
			cout << "|-------------------------|\n";
			cout << "| Play:                   |\n";
			cout << "| - must play highest or  |\n";
			cout << "|  same card (rank)       |\n";
			cout << "| - otherwise MUST play   |\n";
			cout << "|   lowest card in hand   |\n";
			cout << "| - Winner of prior round |\n";
			cout << "|   goes first            |\n";
			cout << "|-------------------------|\n";
			cout << "| Win:                    |\n";
			cout << "| - each player has 30 HP |\n";
			cout << "| - last player standing  |\n";
			cout << "|   (with points) wins    |\n";
			cout << "|-------------------------|\n";
			int returnmenu;
			fail("\nPress any number to return: ", returnmenu);
		} else {
			cout << "Invalid input\n";
		}
	} while (option != 1);
}

void startcards(int& c1, int& c2, int& c3, int& c4, int& c5, int& c6,
                int& p2c1, int& p2c2, int& p2c3, int& p2c4, int& p2c5, int& p2c6,
                int& p3c1, int& p3c2, int& p3c3, int& p3c4, int& p3c5, int& p3c6) {

	int card[52];
	for (int i = 0; i < 52; i++) card[i] = i + 1;

	for (int i = 51; i > 0; i--) {
		int j = rand() % (i + 1);
		int temp = card[i];
		card[i] = card[j];
		card[j] = temp;
	}

	c1 = card[0];
	c2 = card[1];
	c3 = card[2];
	c4 = card[3];
	c5 = card[4];
	c6 = card[5];

	p2c1 = card[6];
	p2c2 = card[7];
	p2c3 = card[8];
	p2c4 = card[9];
	p2c5 = card[10];
	p2c6 = card[11];

	p3c1 = card[12];
	p3c2 = card[13];
	p3c3 = card[14];
	p3c4 = card[15];
	p3c5 = card[16];
	p3c6 = card[17];
}

void ArtsP1(int& card, int& c1, int& c2, int& c3, int& c4, int& c5, int& c6,
            string& c1art, string& c2art, string& c3art, string& c4art, string& c5art, string& c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {

	ClA = "|=====|\n|c    |\n|  A  |\n|    c|\n|=====|\n";
	Cl2 = "|=====|\n|c    |\n|  2  |\n|    c|\n|=====|\n";
	Cl3 = "|=====|\n|c    |\n|  3  |\n|    c|\n|=====|\n";
	Cl4 = "|=====|\n|c    |\n|  4  |\n|    c|\n|=====|\n";
	Cl5 = "|=====|\n|c    |\n|  5  |\n|    c|\n|=====|\n";
	Cl6 = "|=====|\n|c    |\n|  6  |\n|    c|\n|=====|\n";
	Cl7 = "|=====|\n|c    |\n|  7  |\n|    c|\n|=====|\n";
	Cl8 = "|=====|\n|c    |\n|  8  |\n|    c|\n|=====|\n";
	Cl9 = "|=====|\n|c    |\n|  9  |\n|    c|\n|=====|\n";
	Cl10 = "|=====|\n|c    |\n| 10  |\n|    c|\n|=====|\n";
	ClJ = "|=====|\n|c    |\n|  J  |\n|    c|\n|=====|\n";
	ClQ = "|=====|\n|c    |\n|  Q  |\n|    c|\n|=====|\n";
	ClK = "|=====|\n|c    |\n|  K  |\n|    c|\n|=====|\n";

	SA = "|=====|\n|s    |\n|  A  |\n|    s|\n|=====|\n";
	S2 = "|=====|\n|s    |\n|  2  |\n|    s|\n|=====|\n";
	S3 = "|=====|\n|s    |\n|  3  |\n|    s|\n|=====|\n";
	S4 = "|=====|\n|s    |\n|  4  |\n|    s|\n|=====|\n";
	S5 = "|=====|\n|s    |\n|  5  |\n|    s|\n|=====|\n";
	S6 = "|=====|\n|s    |\n|  6  |\n|    s|\n|=====|\n";
	S7 = "|=====|\n|s    |\n|  7  |\n|    s|\n|=====|\n";
	S8 = "|=====|\n|s    |\n|  8  |\n|    s|\n|=====|\n";
	S9 = "|=====|\n|s    |\n|  9  |\n|    s|\n|=====|\n";
	S10 = "|=====|\n|s    |\n| 10  |\n|    s|\n|=====|\n";
	SJ = "|=====|\n|s    |\n|  J  |\n|    s|\n|=====|\n";
	SQ = "|=====|\n|s    |\n|  Q  |\n|    s|\n|=====|\n";
	SK = "|=====|\n|s    |\n|  K  |\n|    S|\n|=====|\n";

	DA = "|=====|\n|D    |\n|  A  |\n|    D|\n|=====|\n";
	D2 = "|=====|\n|D    |\n|  2  |\n|    D|\n|=====|\n";
	D3 = "|=====|\n|D    |\n|  3  |\n|    D|\n|=====|\n";
	D4 = "|=====|\n|D    |\n|  4  |\n|    D|\n|=====|\n";
	D5 = "|=====|\n|D    |\n|  5  |\n|    D|\n|=====|\n";
	D6 = "|=====|\n|D    |\n|  6  |\n|    D|\n|=====|\n";
	D7 = "|=====|\n|D    |\n|  7  |\n|    D|\n|=====|\n";
	D8 = "|=====|\n|D    |\n|  8  |\n|    D|\n|=====|\n";
	D9 = "|=====|\n|D    |\n|  9  |\n|    D|\n|=====|\n";
	D10 = "|=====|\n|D    |\n| 10  |\n|    D|\n|=====|\n";
	DJ = "|=====|\n|D    |\n|  J  |\n|    D|\n|=====|\n";
	DQ = "|=====|\n|D    |\n|  Q  |\n|    D|\n|=====|\n";
	DK = "|=====|\n|D    |\n|  K  |\n|    D|\n|=====|\n";

	HA = "|=====|\n|H    |\n|  A  |\n|    H|\n|=====|\n";
	H2 = "|=====|\n|H    |\n|  2  |\n|    H|\n|=====|\n";
	H3 = "|=====|\n|H    |\n|  3  |\n|    H|\n|=====|\n";
	H4 = "|=====|\n|H    |\n|  4  |\n|    H|\n|=====|\n";
	H5 = "|=====|\n|H    |\n|  5  |\n|    H|\n|=====|\n";
	H6 = "|=====|\n|H    |\n|  6  |\n|    H|\n|=====|\n";
	H7 = "|=====|\n|H    |\n|  7  |\n|    H|\n|=====|\n";
	H8 = "|=====|\n|H    |\n|  8  |\n|    H|\n|=====|\n";
	H9 = "|=====|\n|H    |\n|  9  |\n|    H|\n|=====|\n";
	H10 = "|=====|\n|H    |\n| 10  |\n|    H|\n|=====|\n";
	HJ = "|=====|\n|H    |\n|  J  |\n|    H|\n|=====|\n";
	HQ = "|=====|\n|H    |\n|  Q  |\n|    H|\n|=====|\n";
	HK = "|=====|\n|H    |\n|  K  |\n|    H|\n|=====|\n";

	int cards[6]    = {c1, c2, c3, c4, c5, c6};
	string* arts[6] = {&c1art, &c2art, &c3art, &c4art, &c5art, &c6art};

	for (int i = 0; i < 6; i++) {
		int cardVal = cards[i];
		string art = lookupArt(cardVal,
		                       ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
		                       SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
		                       DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
		                       HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
		*arts[i] = art;
		cout << art;
	}
}

void ArtsP2(int& card, int& p2c1, int& p2c2, int& p2c3, int& p2c4, int& p2c5, int& p2c6,
            string& p2c1art, string& p2c2art, string& p2c3art, string& p2c4art, string& p2c5art, string& p2c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {

	ArtsP1(card, p2c1, p2c2, p2c3, p2c4, p2c5, p2c6,
	       p2c1art, p2c2art, p2c3art, p2c4art, p2c5art, p2c6art,
	       ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
	       SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
	       DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
	       HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
}

void ArtsP3(int& card, int& p3c1, int& p3c2, int& p3c3, int& p3c4, int& p3c5, int& p3c6,
            string& p3c1art, string& p3c2art, string& p3c3art, string& p3c4art, string& p3c5art, string& p3c6art,
            string& ClA, string& Cl2, string& Cl3, string& Cl4, string& Cl5, string& Cl6, string& Cl7, string& Cl8, string& Cl9, string& Cl10, string& ClJ, string& ClQ, string& ClK,
            string& SA, string& S2, string& S3, string& S4, string& S5, string& S6, string& S7, string& S8, string& S9, string& S10, string& SJ, string& SQ, string& SK,
            string& DA, string& D2, string& D3, string& D4, string& D5, string& D6, string& D7, string& D8, string& D9, string& D10, string& DJ, string& DQ, string& DK,
            string& HA, string& H2, string& H3, string& H4, string& H5, string& H6, string& H7, string& H8, string& H9, string& H10, string& HJ, string& HQ, string& HK) {

	ArtsP1(card, p3c1, p3c2, p3c3, p3c4, p3c5, p3c6,
	       p3c1art, p3c2art, p3c3art, p3c4art, p3c5art, p3c6art,
	       ClA, Cl2, Cl3, Cl4, Cl5, Cl6, Cl7, Cl8, Cl9, Cl10, ClJ, ClQ, ClK,
	       SA, S2, S3, S4, S5, S6, S7, S8, S9, S10, SJ, SQ, SK,
	       DA, D2, D3, D4, D5, D6, D7, D8, D9, D10, DJ, DQ, DK,
	       HA, H2, H3, H4, H5, H6, H7, H8, H9, H10, HJ, HQ, HK);
}






