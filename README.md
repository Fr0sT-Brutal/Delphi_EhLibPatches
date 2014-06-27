Патчи для EhLib 3.6
-------------------

Хранятся в дефолтном формате git-format-patch, это Unix mailbox с темой, взятой из текста коммита, и телом письма, составляющим скрипт для diff. Файл открывается в почтовиках типа Outlook, если переименовать его в *.eml.

Ниже следует перечень коммитов с описанием

--- 1 ---
=========

**DBGridEh.pas:**

`!` TColumnEh.CheckboxNullAsFalse, если True, то NULL значения полей будут отображаться как unchecked

**DbUtilsEh.pas:**

`+` Переменная SQLFieldNameQuoteChars, можно менять или обнулять, чтобы экранирования имен полей не было. Используется в GetOneExpressionAsLocalFilterString

`!` ApplySortingForSQLBasedDataSet, исправлено неверное положение указателя сортировки

--- 2 ---
=========

**EhLibZeos.pas:**

`+` Добавлена поддержка сортировки/фильтрации для Zeos Dataset

--- 3 ---
=========

**DclEhLib70.dpk, EhLib70.dpk:**

`*` Изменены пути в файлах пакетов (не придется прописывать ..\Common в путях)

--- 4 ---
=========

**DBGridEh.pas:**

`+` TCustomDBGridEh.InplaceSearchColumn, позволяет указывать стобец, по которому будет выполняться инкрементальный поиск. В основном для использования с опцией FullRowSelect.

--- 5 ---
=========

**DBGridEh.pas:**

`+` TCustomDBEditEh.EmptyAsNull - флаг, при установке которого очищение текста в редакторе присваивает связанному полю NULL вместо пустой строки. Актуален для TDBComboBoxEh и TDBEditEh. TDBDateTimeEditEh и TDBNumberEditEh уже имеют такой функционал

--- 6 ---
=========

**DBCtrlsEh.pas:**

`+` TCustomDBEditEh.ScrollBars. Теперь это практически полноценная замена TDBMemo
