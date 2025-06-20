# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

## Run Locally

**Prerequisites:**  Node.js

1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`


## Run Online

1. echo "VITE_API_KEY=" > .env
2. npm run build
3. git init
4. git add .
5. git commit -m "Integrate Vite build process and restructure project, published for video <Atomic Habits>"

**Prerequisites:** Github创建新的repository
6. git remote add origin https://github.com/Edelweiss-myt/lanlearner_public.git    # git remote remove origin
7. git branch -M main
8. git push origin main        #此时你的github应该也已更新完成

** Netlify **
npm run build
dist
VITE_API_KEY=AIzaSyAY1JopshkJP70BA6YASSw2x8dkyV_AcJk


## Update Online

1. # If needed, npm install , rm package-lock.json, rm -rf node_modules
2. npm run dev
   
3. npm run build, if needed, npm i --save-dev @types/node
4. git branch
5. git add . 
6. git commit -m "Your commit message"
7. git status  # should be 'no changes added to commit'
8. git remote -v   # if incorrect github web, git remote remove origin # git remote add origin https://github.com/Edelweiss-myt/lanlearner_v2.git 
9. git push origin main --force-with-lease
    If failed, git branch --set-upstream-to=origin/main main, git pull, git push


### Version Update
1. '复习' section: 'Add 'Edit' to word, separate 'word' and 'knowledge' when showing all
2. Update ebook (format: word, pdf, epub), the examples of added words will be first searched from ebook, then online resources
3. Automatically save data excel in browser's saving location every week
4. ‘复习-显示全部-单词’分栏添加查询框 (如输入‘a’，则显示所有a开头的单词）
5. 导入数据时防止冗余（以标题为参照，重复内容以更久的日期为准）
6. 单词释义例句查询/选取后可编辑
7. 定义在书中查到>5 标记处，标记为高频词，单词颜色设置为深红色
8. 24h内删除的记录可追回，‘最近删除’按钮放在底栏
