# Keyboard layouts for macOS&Windows by Whiskeroff
Две раскладки клавиатуры (английская и русская) для операционных систем macOS и Windows.

## Причина создания

В интернете куча информации о том как создать свою раскладку. Причины у всех людей разные. Я создавал свои из следующих соображений:

- раскладки клавиатур и маркировка кнопок сильно отличаются для Windows и macOS. Так как я использую обе операционные системы, первую для работы вторую для хобби, то становилось крайне не удобно постоянно подстраиваться под "текущую" ОС;
- я также использую разные клавиатуры, в том числе и Apple. Хотелось бы, что бы их поведение было максимально унифицировано;
- не хватает быстро набираемых дополнительных символов, опять же в обеих ОС.

## Основные идеи

1. Все комбинации должны работать одинаково для macOS и Windows .
2. Дополнительные и специальные символы должны набираться однинаково и в русской и в английской раскладке.
3. Расширить набор быстро набираемых дополнительный символов за счет комбанаций с клавишей Option(AltGr).

Все идеи отразил на такой схеме:
![keyboard](/Images/WhiskKBLayouts.png)
, исходник схемы в Excel находится в папке _**Images**_.
Также в папке _**Images**_ находятся PDF-ки полученные в использованных программах.

Далее описание использования раскладки, по трем типам клавиш (см. схему выше):

![keys_row_num](/Images/keys_row_num.png)
![keys_row_alpha](/Images/keys_row_alpha.png)

## Реализация
1. Буква ё/Ё находится слева вверху в русской раскладке.
2. Ряд цифровых клавиш 1234567890-= использует символы русской раскладки на Windows (т.к. я чаще работаю с русской расскладкой), символы английской раскладки спрятаны в комбинацию с Option(AltGr). "Пустые" места клавиш 90-=, заполнены дополнительными символами.
3. Несмотря на то, что я оставил точку и запятую в английской расладке на своих местах, я стараюсь ими не пользоваться, для этого есть клавиша слева от правого Shift, которая работает одинаково во всех раскладках. На ней же "висит" и многоточие.
4. Переделал кнопку с обратным слешем, теперь там три символа: slash/backslash/pipe.
5. На моей схеме есть кнопка справа от левого Shift, она присутствует на клавиатурах формата ISO. У меня две клавиатуры ISO и две ANSI, поэтому я решил отказаться от использования этой клавиши, что бы не превыкать.
6. Обратите внимание, даже на клавиатурах Apple я сохраняю порядок клавиш нижнего ряда как у клавиатур Windows, macOS позволяет легко это настроить. Control-Fn(при наличии)-Command(Windows)-Option(Alt)-Space-Option(AltGr)-Menu(при наличии)-Control. Такми образом мне не нужно перестраивать при смене компьютера и операционной система.
7. Самый большой блок клавиш латинской раскладки A÷Z в комбинации с Option(AltGr):
        
    7.1 Для работы мне нужны виды излучений: A-α, B-β, G-γ;
    
    7.2 Символы для римских цифр всегда под рукой, даже на русской раскладке: I,V,X,L;
    
    7.3 Технические символы: G-°(градус), O-Ø(диаметр), P-π(пи), S-§(параграф), U-µ(микро), Z-√(квадратный корень);
    
    7.4 C-©(Copyright), R-®(Registerd Trademark), T-™(Trade Mark), D-$(Dollar), E-€(Euro);
    	
    7.5 Символы Apple: H-(control), J-(cmd), K-(option), N-(shift), M-(Apple).

## Инструменты (программы)

Исходные пакеты размещены в папке _**Layouts**_:
- для macOS использовалась известная программа [Ukekele](http://software.sil.org/ukelele/) version 3.4.2 (3.4.2.314), в одном пакете две раскладки: "EN by Whisk" и "RU by Whisk";
- для создания инсталяторов для Windows использовалась программа [Microsoft  Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=22339) version 1.4.

## Перечень раскладок

- macOS:
  - EN by Whisk;
  - RU by Whisk;
- Windows:
  - Английская - EN Whisk;
  - Русская - RU Whisk.
  
## Установка

- macOS: открыть образ *.dmg, использовать приложение **"Keyboard Installer.app"** для установки **"WhiskKBLayouts.bundle"** либо вручную скопировать пакет в _**/Library/Keyboard Layouts**_ (для всех пользователей) или в _**~/Library/Keyboard Layouts**_ (только для текущего пользователя).
- Windows: распаковать *.zip архив, запустить установщик, каждая раскладка в отдельном архиве.
