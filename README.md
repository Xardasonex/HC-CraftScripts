# HC-CraftScripts

![Hex-Craft Logo](https://hex-craft.ru/templates/Standart/img/hexcraft.svg "Hex-Craft Logo")

Файл скрипта - .zs

Почти все названия предметов можно посмотреть в файлик MinecraftItems.log

Для смены разметки в Notepad++ Синтаксис -> Пользовательский -> Задать -> Импортировать и CraftScript.xml

Как сделать крафт:

Если предмет который будет крафтиться используется в других крафтах, нужно записать его в предметах в таком виде:
val itemName = <ic2:item:3>;

Сам крафт:
recipes.addShaped("НазваниеКрафта", предмет_крафта,
 [[null,		iron,			null],
  [ironPlate,	ironPlate,		ironPlate],
  [null,		ironFurnance,	null]]);

recipes.addShaped - функция добавления форменного рецепта, название крафта в кавычках, имя предмета(которое уже прописано), и предметы по каждой ячейке, null - пустая ячейка, табуляция не обязательна, сделал для наглядности.

---

 Сделано для лучшего майнкрафт проекта HexCraft. https://hex-craft.ru
