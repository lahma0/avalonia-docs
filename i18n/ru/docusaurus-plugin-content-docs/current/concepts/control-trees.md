---
description: CONCEPTS
---

import ControlTreesLogicalScreenshot from '/img/gitbook-import/assets/image (61).png';
import ControlTreesVisualScreenshot from '/img/gitbook-import/assets/image (15) (2).png';
import ControlTreesEventScreenshot from '/img/gitbook-import/assets/image (1) (1) (2).png';

# Деревья элементов

_Avalonia UI_ создает деревья элементов из XAML-файлов приложения. Они отвечают за вывод элементов интерфейса и управляют их функциональностью.

## Логические деревья

Логические деревья являются иерархическим представлением элементов приложения (включая основное окно), определенных в XAML-файлах.
К примеру, у нас есть окно, а в нем определен некий элемент, внутри которого есть элемент `Кнопка`. Тогда будет построено следующее логическое дерево:

<img src={ControlTreesLogicalScreenshot} alt=""/>

Если ваще приложение запущено, то после нажатия кнопки "F12", появится окно _Avalonia Dev Tools_. В нем можно найти логическое дерево во вкладке **Logical Tree**.

## Визуальное дерево

Визуальное дерево элементов управления содержит все, что на самом деле отоброжается в _Avalonia UI_. Оно показывает все свойства, установленные для элементов управления, и все дополнительные части, которые были добавлены _Avalonia UI_ для представления пользовательского интерфейса и управления функциональностью приложения. Основное отличие от логичесого дерева - визуальное дерево также включает скрытые составляющие шаблонов элементов. 

<img src={ControlTreesVisualScreenshot} alt=""/>

Визульное дерево можно увидеть на вкладке **Visual Tree** в окне _Avalonia Dev Tools_.

## События

Важной частью управления функциональностью приложения, осуществляемого _Avalonia UI_, является вызов и обработка событий. На вкладке **Events** регистрируются источники и обработчики событий при перемещении и ином взаимодействии с запущенным приложением.

<img src={ControlTreesEventScreenshot} alt=""/>