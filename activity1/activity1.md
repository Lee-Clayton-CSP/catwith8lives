1. less +3 billboard.tsv
2. sort -r -n billboard.tsv | less
3. cut -f 3 billboard.tsv | less
4. "grep "Justin" billboard.tsv | wc -l": 13
5. "cut -f 3 billboard.tsv | sort -f -u | wc -l": 91
6. "cut -f 3 billboard.tsv | sort -f | uniq -c | sort -n -r": Justin Bieber
7. cut -f 2 billboard.tsv | less
8. "cut -f 2 billboard.tsv | tr ' ' '\n' | sort -f | uniq -c | sort -n -r": you
9. sort -m a b | sort -u -f > c
10. comm -12 <(sort a) <(sort b) > c

Note on 5: We are aware that artists featuring someone else counts as unique from them singing alone, but we have yet to learn a way to alleviate that.