# Joel Ayitevi01244229d
#include <cstdlib>
#include <iostream>

using namespace std;

int main(int argc, char *argv[])
#include <iostream>
#include <vector>
#include <string>
#include <algorithm>
using namespace std;

// 1. Sum of two integers
int sum(int x, int y) {
    return x + y;
}

// 2. Count vowels in a string
int countVowels(string s) {
    int count = 0;
    for (char c : s) {
        c = tolower(c);
        if (c=='a'||c=='e'||c=='i'||c=='o'||c=='u')
            count++;
    }
    return count;
}

// 3. Average of integers
double average(vector<int> nums) {
    int total = 0;
    for (int n : nums)
        total += n;
    return (double)total / nums.size();
}

// 4. Remove vowels from sentence
string removeVowels(string s) {
    string result = "";
    for (char c : s) {
        char lower = tolower(c);
        if (!(lower=='a'||lower=='e'||lower=='i'||lower=='o'||lower=='u'))
            result += c;
    }
    return result;
}

// 5. Longest string in list
string longestString(vector<string> words) {
    string longest = words[0];
    for (string w : words) {
        if (w.length() > longest.length())
            longest = w;
    }
    return longest;
}

// 6. Median of integers
double median(vector<int> nums) {
    sort(nums.begin(), nums.end());
    int n = nums.size();
    if (n % 2 == 0)
        return (nums[n/2 - 1] + nums[n/2]) / 2.0;
    else
        return nums[n/2];
}

// 7. Remove even numbers
vector<int> removeEven(vector<int> nums) {
    vector<int> result;
    for (int n : nums) {
        if (n % 2 != 0)
            result.push_back(n);
    }
    return result;
}

// 8. Sort strings alphabetically
vector<string> sortStrings(vector<string> words) {
    sort(words.begin(), words.end());
    return words;
}

// 9. Sum of list of integers
int sumList(vector<int> nums) {
    int total = 0;
    for (int n : nums)
        total += n;
    return total;
}

// 10. Reverse strings in list
vector<string> reverseStrings(vector<string> words) {
    for (string &w : words)
        reverse(w.begin(), w.end());
    return words;
}
    system("PAUSE");
    return EXIT_SUCCESS;
}
