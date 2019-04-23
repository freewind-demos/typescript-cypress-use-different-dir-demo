TypeScript Cypress Use Different Dir Demo
=========================================

cypress默认使用的是项目下`cypress`这个目录，如果想换个目录，可能因为cypress的问题，并没有那么简单。

虽然 https://docs.cypress.io/guides/references/configuration.html#Folders-Files 中提供了
`fileServerFolder`这个选项，看似是指定整体目录，但是没用，还必须依次指定其它各项目录或者文件，
否则运行`cypress open`时，会自动创建`cypress`及相应的子目录。

未来可能会增加`cypress init`命令来解决相关问题：
https://github.com/cypress-io/cypress/issues/619

```
npm install
npm run test:open
npm run test:run
```
