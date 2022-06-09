#Branches
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

git branch Postman
git branch Jmeter
git branch CheckLists
git branch Bag Reports
git branch SQL
git branch Charles
git branch Mobile testing

2. Запушить все ветки на внешний репозиторий
git push --all
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
 git checkout Bag_reports
 cat > Bag_reports.txt
4. Запушить структуру багрепорта на внешний репозиторий
 git add Bag_reports.txt
 git commit -m "add Bag"
 git push -u origin Bag_reports
5. Вмержить ветку Bag Reports в Main
 git checkout main
 git merge Bag_reports -m "merge Bag"
6. Запушить main на внешний репозиторий.
 git push
7. В ветке CheckLists набросать структуру чек листа.
 git checkout CheckList
 cat > ChckLst.txt 
8. Запушить структуру на внешний репозиторий
 git add ChckLst.txt
 git commit -m "add ChckFile"
 git push -u origin CheckList
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main
 git checkout main
 git fetch
 git pull
