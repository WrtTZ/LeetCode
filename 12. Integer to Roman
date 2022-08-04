class Solution {
public:
    string intToRoman(int num) {
        int quo = 0;
        string r = "";
        vector<int> numbers{1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1};
        vector<string> romans{"M", "CM", "D", "CD", "C", "XC", "L", "XL", "X", "IX", "V", "IV", "I"};
        
        for (int i = 0; i < 13; i++) {
            if (num >= numbers[i]) {
                quo = num / numbers[i];
                num = num % numbers[i];
                
                while (quo > 0) {
                    r += romans[i];
                    quo--;
                }
            }
        }
        
        return r;
    }
};
