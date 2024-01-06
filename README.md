# Number-of-Newtons
Number of Newtons  Given a string, find how many "newton" can be formed using the characters of the given string.   Input Input consists of a string, s ( 1 &lt;= |s| &lt;= 105) Output Output an integer, the number of "newton".

def count_newton_occurrences(s):
    letter_counts = {
        'n': s.count('n'),
        'e': s.count('e'),
        'w': s.count('w'),
        't': s.count('t'),
        'o': s.count('o'),
    }

    return min(letter_counts.values())

if __name__ == "__main__":
    try:
        s = input().strip()
        result = count_newton_occurrences(s)
        print(result)
    except EOFError:
        pass

