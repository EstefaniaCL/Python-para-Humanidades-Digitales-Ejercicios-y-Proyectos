#PRIMERA VERSIÓN
autor="Charlotte Brontë"
titulo="Jane Eyre"
año=1847#Python no mete enteros en una cadena, hay que convertirlo con str
lugar="Reino Unido"

print(autor+". "+(titulo)+ ". "+str(año)+". "+(lugar)+".")

#SEGUNDA VERSIÓN
Cita=f"{autor}. {titulo}. {año}. {lugar}."#Aquí ya no hay que convertir el año
print(Cita)

#Cursiva
Cita2=f"{autor}. *{titulo}*. {año}. {lugar}."

#CALCULAR EDAD DE LA OBRA
año_actual=2026
edad_obra=año_actual-año
print(f"{titulo} tiene {edad_obra} años de antiguedad.")

#VARIOS AUTORES
first_author = "Diderot"
second_author = "d'Alembert"
title = "Encyclopédie"
year = 1751

citation = f"{first_author} and {second_author}. *{title}*. {year}."
print(citation)

#LIMPIEZA DE LOS DATOS
raw_author = "  voltaire  "
raw_title = "candide"

author=raw_author.strip().title()    # "Voltaire"
title =raw_title.title()              # "Candide"

print(f"{author}. *{title}*.")

#COMPLETO
raw_author = "  voltaire  "
raw_title = "candide"
year = 1759
place = "Paris"
current_year = 2025

author = raw_author.strip().title()
title = raw_title.title()
age = current_year - year

citation = f"{author}. *{title}*. {year}. {place}."
print(citation)
print(f"This work is {age} years old.")
