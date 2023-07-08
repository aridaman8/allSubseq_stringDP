# allSubseq_stringDP

void printSubsequence(string input, string output)
{
    if (input.empty()) {
        cout << output << endl;
        return;
    }
    printSubsequence(input.substr(1), output + input[0]);
 
    printSubsequence(input.substr(1), output);
}
//  intput is original string
// output is a empty string
