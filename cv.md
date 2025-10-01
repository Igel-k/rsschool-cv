# Karina Sedova

## Contact information
- Location: Moscow, Russia
- email: karina.sed@yandex.ru
- GitHub: [Igel-k](https://github.com/Igel-k)

## About me
I am responsible, sociable, punctual, motivated and well organized. I can work both in a team and independently. I am constantly in search of new knowledge and skills. I am able to work under tight deadlines and meet deadlines.

## Skills
- C/C++, OpenMP, MPI
- Python, Django
- JavaScript, React
- HTML, CSS
- Git

## Code example
Python. Task [Diagonal decode](https://www.codewars.com/kata/55af0d33f9b829d0a800008d/)

```python
def get_diagonal_code(grid):
    by_lines = list(grid.split("\n"))

    by_letters = []
    for line in by_lines:
        by_letters.append(list(line.split(" ")))
    
    counter = 0
    direction = 'to bot'
    flag = False
    result = []

    current_lines = by_letters.copy()
    
    if len(current_lines) == 1:
        return current_lines[0][0]

    while not flag:
        if direction == 'to bot':
            for line in current_lines:
                if len(line) > counter:
                    result.append(line[counter])
                    counter += 1
                else:
                    flag = True
                    break
            direction = 'to top'
            current_lines = by_letters.copy()
            current_lines.reverse()
            del current_lines[0]
        elif direction == 'to top':
            for line in current_lines:
                if len(line) > counter:
                    res_string.append(line[counter])
                    counter += 1
                else:
                    flag = True
                    break
            current_lines = by_letters.copy()
            del current_lines[0]
            direction = 'to bot'

    res_string = ''.join(map(str, res_string))
    return res_string
```

## Experience
- [rsschool-cv](https://github.com/Igel-k/rsschool-cv/)

## Education
- **University**: Bauman Moscow State Technical University, Apllied Mathematics (2018 -- 2024)
- **Course**: Professional retraining course (BMSTU), Web-deveploment (2022 -- 2023)

## Languages
- Russian: Native
- English: Intermediate
- German: Pre-Intermediate