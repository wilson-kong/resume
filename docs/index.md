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
    - [She codes](#she-codes)
    - [Software Engineer - Teaching Assistant](#software-engineer---teaching-assistant)
  - [Projects](#projects)
  - [Volunteer experience](#volunteer-experience)

## Education
| BE/ME |  UQ |
| :---------------- | ----: |
| Majoring in Mechatronics ||

```bash
BE/ME |  UQ
```

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

    def __str__(self) -> str:
        """ Return the role description """
        print(f'Work as a {self._title} at {self._company} '\
        'located in {self._location} '
        'from {duration[0]} to {duration[1]}.')
```
### She codes
```python
>>> duration = (2023, 'present')
>>> work = Work(
        'Software Mentor - Python(Django, DRF)',
        'She Codes',
        duration,
        'Brisbane'
    )
>>> print(work)
```

### Software Engineer - Teaching Assistant
```python
>>> duration = (2019, 'present')
>>> work = Work(
        'Software engineer - Teaching assistant',
        'The University of Queensland',
        duration,
        'Brisbane'
    )
>>> print(work)
```

## Projects
* [Wordle Clone](https://wilson-kong.github.io/games)

## Volunteer experience

<!-- ## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files. -->

