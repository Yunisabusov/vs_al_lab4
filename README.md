# Birinci məsuliyyət: Ədədi massivi yaratmaq və fayla yazmaq
ededi_massiv = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

with open('ededler.txt', 'w') as fayl:
    for eded in ededi_massiv:
        fayl.write(str(eded) + '\n')

# İkinci məsuliyyət: Cüt ədələri tapmaq və yeni fayla yazmaq
cut_ededler = [eded for eded in ededi_massiv if eded % 2 == 0]

with open('cut_ededler.txt', 'w') as cut_fayl:
    for cut_eded in cut_ededler:
        cut_fayl.write(str(cut_eded) + '\n')

# Üçüncü məsuliyyət: Cüt ədələrin cəmini hesablayıb çap etmək
cut_ededler_cemi = sum(cut_ededler)
print(f'Cüt ədələrin cəmi: {cut_ededler_cemi}')
