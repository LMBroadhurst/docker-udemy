```bash
docker run 9c7a7aa608c9b9eb6deeadf07460effb4bd42255681531702464bbef96713588
# Enter the minimum number: Traceback (most recent call last):
#   File "/app/rng.py", line 3, in <module>
#     min_number = int(input("Enter the minimum number: "))
#                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
# EOFError: EOF when reading a line

# Needs to be 'interactive' and also useful to have a terminal...
docker run --help

docker run -it 9c7a7aa608c9b9eb6deeadf07460effb4bd42255681531702464bbef96713588
# Enter the minimum number: 5
# Enter the minimum number: 10
# Random number between 5 and 10 is 5

# For docker start...
docker start -ai 9c7a7aa608c9b9eb6deeadf07460effb4bd42255681531702464bbef96713588
```