# test_previewlimitsize
What is the limit size of text not to be previewed on GitHub.com repo?

## Result
- [1MB](1MB.py) :x:
- [1MB-1B](1MB-1B.py) :o:

## Steps
- 1. `1024*1024-(24+1) = 1048551`
- 2. `python -c "print 'a'*1048551" > 1048551.txt`
- 3. Add the content of 2. to skeleton.py
