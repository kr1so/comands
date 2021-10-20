# команды GIT для работы и плюшки

git config --global usern.name - имя
git config --global user.email - имейл
git config --global colour.ni auto - подчеркивать ошибки
git config --list - проверка изменений
ls - показать список файлов
cd (название папки/файла) - выбрать папку/файл
cd .. - переход в папку уровня выше
cd ../.. - переход в папку на 2 уровня выше
mkdir - создать директорию
touch - создать папку/файл
cp (название копируемого файла) (название файла в который хотим скопировать) - копировать файлы
mv (файл, который хотим переименовать) (файл, в который хотим переименовать) - переименовать файлы
echo "(слово)" - записать информацию
echo "(слово)" > (файл) - записать информацию в файл
cat (название файла) - посмотреть содержимое файла
rm (название файла) - удалить файлы
rm -r (название директории) - удалить директорию
git init - из пустого репозитория в текущее местоположение
ls -a - показать все файлы, в т.ч. скрытые
git status - текущее состояние репозитория
git remote add origin - добавить удаленный источник данных
git remote -v - подключение соединения
git rm --cashed (название файла) - удалить из коммита
git commit - создать коммит
i - для записи изменений инфо в коммите
:wq (клавиша enter) - сохранить текущий буфер и закрыть его
:git add <(файл)> - добавить файл к текущему
git commit - записать коммит
git commit -m '(сообщение коммита)' - записать коммит с сообщение
git log - история репозитория
git log -oneline - история репозитория в компактном виде
git reset (хэш коккита) - вернуться на состояние предыдущего коммита
git reflog - подробные изменения всех операций в репозитории
git revert - создание нового коммита, отмена действия, совершенное в предыдущем коммите
git restore - сброс состояния файла на указанное
git branch - доступные ветки
git branch (название ветки) - создать ветку
git checkout (название ветки) - переключение между ветками
git add (название файла) - добавить в индекс репозитория
git checkout -b (название ветки) - создать ветку в рамках текущей ветки или переключиться
ssh-keygen - генерация ключа ssh-подключения
git clone - скопировать
git push - загрузить изменения 
git push -u - загрузить изменения с текущей ветки на удаленную
git pull - загрузить все изменения коммита в ветку
git fetch - подгрузить обновления из репозитория
clear - очистить терминал
git push u origin (название ветки) - из локального репозитория в гитхаб
git branch --merged (название ветки) - какие ветки слиты в выбранной веткой
git branch --no merged (название ветки) - какие ветки не слиты с выбранной веткой
git branch -D (имя ветки) - удалить ветку
git push --force - принудительная перезапись состояния удаленного репозитория на текущий
rm -rf (название файла/репозитория) - принудительное удаление каталога и всех его файлов
git branch (название новой ветки) (название прикрепленной ветки) - создать новую ветку от основной ветки
git push --set-upstream origin (название ветки) - загрузить изменения в автоматическом режиме с текущей на origin (удаленную)
git branch -vv - просмотр привязанных веток
git merge (название ветки)-замержить ветки
git push --delete origin (название ветки) - удалить ветку с гитхаб
git rebase (название ветки) - сместить на последний коммит другой ветки
git tag (номер версии, 1.0.1, например) - версия изменений
git tag - проверка коммита версии
git tag --list - проверка остальных тегов
git push --tags - загрузить изменения тегов в удаленный репозиторий
git tag -d (номер тега) - удалить прошлую версию
git push --delete origin - удаление тегов с удаленного репозитория
git stash - использовать временное хранилище для несохраненных файлов
git stash list - доступные стэши
git stash push (название файла) - добавить изменения в уже существующий стэш
git stash pop (название стэша) - применить изменения из стэша на нужную ветку
git merge (название ветки) --squash - объединить все коммиты, чтобы записать один на основной ветке
git reset --hard
git rebase HEAD~(количество коммитов, которые хотим объединить) - склеить коммиты
git rebase - i HEAD~(количество коммитов, которые хотим объединить)
git log --oneline --all - просмотр всех изменений веток
git cherry-pick (хэш коммита, который хотим перенести) - перенести отдельный коммит
git cherry-pick (название ветки) - перенести последний коммиит ветки
git cherry-pick ..(название ветки) - перенести все коммиты ветки
git commit --amend - перезаписать коммит
vi (название файла) - исправить конфликт, просмотр файла

git add * - добавить все файлы в репозиторий
git add *.md - добавить файлы с определенным расширением, в данном примере ".md"
git diff - показать разницу между версиями файла (работает до git add)
git diff --staged - показывает сравнение что станет с файлом перед git commit (сперва сделать git add, затем git diff --staged)
git log --graph - визуальное отображение веток

## Порядок работы с fork репозиторием:
Создание fork
Клонирование
Разработка
Публикация
Создание pull-request (p-r)