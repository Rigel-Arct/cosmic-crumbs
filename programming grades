characters = [
    {'ID': '000630060', 'LAST NAME': 'Abdi', 'FIRST NAME': 'Phillip', 'HOMEWORK': 17, 'TEST': 14, 'JANUARY EXAM': 15},
    {'ID': '000654108', 'LAST NAME': 'Benaissa', 'FIRST NAME': 'Willow', 'HOMEWORK': 20, 'TEST': 17, 'JANUARY EXAM': 15},
    {'ID': '000642084', 'LAST NAME': 'Gelashvili', 'FIRST NAME': 'Kenneth', 'HOMEWORK': 19, 'TEST': 17, 'JANUARY EXAM': 18},
    {'ID': '000618036', 'LAST NAME': 'Hoshino', 'FIRST NAME': 'Mitsi', 'HOMEWORK': 20, 'TEST': 18, 'JANUARY EXAM': 17},
    {'ID': '000636072', 'LAST NAME': 'Kowalski', 'FIRST NAME': 'Liliana', 'HOMEWORK': 20, 'TEST': 16, 'JANUARY EXAM': 16},
    {'ID': '000624048', 'LAST NAME': 'Mujinga', 'FIRST NAME': 'Elaine', 'HOMEWORK': 18, 'TEST': 19, 'JANUARY EXAM': 19},
    {'ID': '000606012', 'LAST NAME': 'Nilsson', 'FIRST NAME': 'Benji', 'HOMEWORK': 20, 'TEST': 20, 'JANUARY EXAM': 16},
    {'ID': '000660120', 'LAST NAME': 'Okonkwo', 'FIRST NAME': 'Virgil', 'HOMEWORK': 14, 'TEST': 10, 'JANUARY EXAM': 12},
    {'ID': '000672144', 'LAST NAME': 'Russo', 'FIRST NAME': 'Ollie', 'HOMEWORK': 20, 'TEST': 18, 'JANUARY EXAM': 17},
    {'ID': '000648096', 'LAST NAME': 'Serik', 'FIRST NAME': 'Tiffany', 'HOMEWORK': 16, 'TEST': 13, 'JANUARY EXAM': 14},
    {'ID': '000666132', 'LAST NAME': 'Walsh', 'FIRST NAME': 'Irene', 'HOMEWORK': 20, 'TEST': 15, 'JANUARY EXAM': 13},
    {'ID': '000612024', 'LAST NAME': 'Zahid', 'FIRST NAME': 'Sylvan', 'HOMEWORK': 15, 'TEST': 15, 'JANUARY EXAM': 14}
    ]

# Homework = 3 pts
# Test = 5 pts
# Exam = 12 pts

def average(students: list[dict]) -> dict:
    averages = {}
    for student in students:
        averages[student['ID']] = {}
        averages[student['ID']]['AVERAGE'] = round(student['HOMEWORK']*0.15 + student['TEST']*0.25 + student['JANUARY EXAM']*0.6, 1)
        if averages[student['ID']]['AVERAGE'] >= 10:
            averages[student['ID']]['PASS?'] = True
        else:
            averages[student['ID']]['PASS?'] = False
    return dict(sorted(averages.items()))

print(average(characters))
