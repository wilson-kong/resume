# Welcome to Wilson
This website is dedicated to outlining my experience and skillsets.
<!-- For full documentation visit [mkdocs.org](https://www.mkdocs.org). -->

<!-- ## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit. -->

- [Welcome to Wilson](#welcome-to-wilson)
  - [Education](#education)
  - [Work experience](#work-experience)
    - [Industry Mentor - Python(Django, DRF)](#industry-mentor---pythondjango-drf)
    - [Software Engineer - Teaching Assistant](#software-engineer---teaching-assistant)
  - [Projects](#projects)
  - [Volunteer experience](#volunteer-experience)

## Education
| BE/ME |  UQ |
| :---------------- | ----: |
| Majoring in Mechatronics ||

--------------------------------------------------
## Work experience
```python
class Work:
    def __init__(self, title: str, company: str, duration: tuple, location: str):
        """ Creates an instance of work.
            Parameters:
                title: Job title.
                company: Company name.
                duration: start and end dates of the role. i.e. (start, end)
                location: Location of job
        """
        self._title = title
        self._company = company
        self._start = duration[0]
        self._end = duration[1]
        self._location = location
        self._responsibilities = []

    def add_responsibility(self, responsibility: str):
        """ Add a responsibility to this role.
            Parameters:
                responsibility: description of responsibility.
        """
        self._responsibilities.append(responsibility)

    def __str__(self) -> str:
        """ Return the role description """
        print(f'Work as a {self._title} at {self._company} '\
        f'located in {self._location} '\
        f'from {duration[0]} to {duration[1]}.')

        print('My key responsibilities include:')
        for responsibility in self._responsibilities:
            print(f'- {responsibility}')
```
### Industry Mentor - Python(Django, DRF)
```python
>>> duration = (2023, 'present')
>>> work = Work(
        'Industry Mentor - Python(Django, DRF)',
        'She Codes',
        duration,
        'Brisbane or Meeanjin'
    )
>>> work.add_responsibility('Python education. Object-oriented programming '\
    'philosophies and best practices.')
>>> work.add_responsibility('Django, DRF, and React mentoring.')
>>> work.add_responsibility('Communicate and mentor adults that have spent '\
    'time in different fields.')
>>> print(work)
```

### Software Engineer - Teaching Assistant
```python
>>> duration = (2019, 'present')
>>> work = Work(
        'Software engineer - Teaching assistant',
        'The University of Queensland',
        duration,
        'Brisbane or Meeanjin'
    )
>>> print(work)
```

--------------------------------------------------
## Projects
* [Wordle Clone](https://wilson-kong.github.io/games)

--------------------------------------------------
## Volunteer experience

<!-- ## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files. -->

