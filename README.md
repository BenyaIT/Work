# Контрольная работа

## Задачи

* Создать репозиторий на GitHub

* Нарисовать блок-схему алгоритма

* Снабдить репозиторий оформленным тестовым описанием решения

* Написать программу, решающую поставленную задачу

* Использовать контроль версий в работе над этим небольшим проектом

1. Создать репозиторий GitHub

Создали репозиторий github.com, затем добавляем все в репозиторий с помощью командд


git init

git remote add origin https://github.com/BenyaIT/Work.git 

git branch -M main

git push -u origin main

2. Нарисовать блок-схему алгоритма

https://app.diagrams.net - с помощью этого сайта создаем блок-схему

3. Снабдить репозиторий оформленным тестовым описанием решения

Для этого задания, был создан файл README.md, который вы и читаете, с использованием языка раметки Markdown

4. Написать программу

string[] array1 = new string[5] {"321", "12", "hello", "world", "hi"};
string[] array2 = new string[array1.Length];

void SecondArrayWithIF(string[] array1, string[] array2)

{
    int count = 0;

    for (int i = 0; i < array1.Length; i++)
    {
    if(array1[i].Length <= 3)
        {
        array2[count] = array1[i];
        count++;
        }
    }
}

void PrintArray(string[] array)

{
    for (int i = 0; i < array.Length; i++)

    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}

SecondArrayWithIF(array1, array2);
PrintArray(array2);

5. Использовать контроль версий в работе над этим небольшим проектом

После каждого пункта делали коммиты командой 

git add .\README.md

git commit -m "текст коммита"

Для отправки изменений в репозиторий  команда

git push