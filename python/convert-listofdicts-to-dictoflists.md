## How to convert list of dicts to dict of lists?

We will use zip for performing this operation

```
student_list = [{"first_name": "Sancheeta", "last_name": "Kaushal", "id": 1},
            {"first_name": "Saksham", "last_name": "Kaushal", "id": 2},
            {"first_name": "Shourya", "last_name": "Mehta", "id": 3},
            {"first_name": "Soumya", "last_name": "Mehta", "id": 4}
            {"first_name": "Shrishti", "last_name": "Mehta", "id": 5}]

student_dict = dict(zip(
                student_list[0], zip(*[d.values() for d in student_list])
               ))

```
