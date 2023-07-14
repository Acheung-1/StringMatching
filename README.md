# StringMatching

FM-index can find short patterns of length m in long texts of length n in O(m) time. This is because the long test is preprocessed in O(nlogn) time.

# Usage Instructions 

# FMindex
Enter text string into  FMindex

# Important attributes
charList = array - alphabetically sorted unique characters within text including $

charSet = dictionary - all unique characters and their number of occurences

suffixArray = array

firstCol = string - characters of the first column of the BWT matrix

lastCol = string - BWT

skip = dictionary - all unique characters and total number of characters that occur before it alphabetically

LF = array - LF mapping

fArray = array with n number of subarrays where n is number of unique characters - subarray is indexed based on order it appears in charList, each subarray contains number of occurences of that character in firstCol[:i] (including i)

lArray = array with n number of subarrays where n is number of unique characters - subarray is indexed based on order it appears in charList, each subarray contains number of occurences of that character in lastCol[:i] (including i)

To match, call function substringMatch(pattern)


### KMP
Enter pattern into KMP
To match, call function substringMatch(text, pattern)


Text and Pattern should only contain the alphabet, no unique characters are allowed
