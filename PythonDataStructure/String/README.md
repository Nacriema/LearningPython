# String in Python

1. Introduction: 
* Python has build-in class called `str` 
* Python strings are "immutable" means that they cannot be changed after they created. 
* Python uses zero-based indexing, if index is out of bounds, Python raises error.


2. String Methods:
* **s.lower(), s.upper()**: Return the lowercase and uppercase version of string
* **s.strip()**: Return a string with whitespace removed from start and end.
* **s.startswith('other'), s.endswith('other')**: test if a string starts or ends with the given other string
* **s.isalpha()/s.isdigit()/s.isspace()...**: Test if all string character starts or ends in various character classes.
* **s.find('other')**: search for the given string within s or not and returns the first index where it begin or -1 if 
not found.
* **s.replace('old', 'new')**: Return a string where all occurrences of 'old' have been replaced by 'new'.
* **s.split('delim')**: Return a list of substrings separated by the given delimiter. The delimiter just the text. Special
case is s.split() then delimiter is **whitespaces** between another characters.
* **s.join(list)**: Opposite of slit(), it joins the elements in the given list using string as delimiter 
> Example: a = 'Huy Truong  Mai'
>
> a.split()  # Return ['Huy', 'Truong', 'Mai']
>
> 'A'.join(a.split())  # Return 'HuyATruongAMai'
>

3. i18n String (Unicode)

* Regular Python string are **not** unicode, they just plain bytes. To create a unicode string, use the 'u' prefix on the 
string literal.

* To convert unicode string to bytes with an encoding such as 'utf-8', call ustring.encode('uft-8').
* To convert encoded plain bytes to a unicode string, use the unicode(s, encoding) (this is old), in Python3: 
use the method s.decode(decode_type). Reason is Python3 the type `unicode` renamed to `str`, the old `str` type rename
to `bytes`

> Example: 
>
> ustring = u'A unicode \u018e string \xf1'
>
> type(ustring) # Return str
>
> ustring # Return  'A unicode Ǝ string ñ'
>
> s = ustring.encode('utf-8')
>
> type(s) # Return bytes
>
> s  # b'A unicode \xc6\x8e string \xc3\xb1'
>
> t = s.decode('utf-8')
>
> type(t) # str
>
> t  # 'A unicode Ǝ string ñ'



 
