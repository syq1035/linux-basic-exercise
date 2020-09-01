请按照流程的每一步书写相应的命令。

1. 请在用户目录下创建一个名称为 cli-practice 的目录。

2. 请在 ~/cli-practice 目录下创建一个空白文件 readme.md。
3. 请在 ~/cli-practice/readme.md 中添加一行文本：Hi there, this is a readme file.
4. 请在 ~/cli-practice/readme.md 中追加一行文本：This is the second line of the readme file.。在这条命令执行完毕之后，~/cli-practice/readme.md 文件中应当包含两行文本。
5. 请将 ~/cli-practice/readme.md 文件改名为 readme.txt
6. 请创建目录 ~/cli-practice/document
7. 请将 ~/cli-practice/readme.txt 文件移动到 ~/cli-practice/document 中，并改名为 introduction.txt。
8. 请将 ~/cli-practice/document 中的 introduction.txt 文件在 ~/cli-practice/document 目录复制一份，并命名为 readme.txt
9. 请使用 The quick brown fox jumps over a lazy dog 这行文本覆盖 ~/cli-practice/document/readme.txt 文件的内容。
10. 请将 ~/cli-practice/document 目录复制到 ~/cli-practice/docs，目录中的文件也要进行复制。
11. 删除 ~/cli-practice/document 目录及其中文件。
12. 请创建 ~/cli-practice/parent/child/docs 目录。
13. 请将 ~/cli-practice/docs/introduction.txt 文件复制到~/cli-practice/parent/child/docs目录下

执行过程：

``` 
mkdir cli-practice
cd cli-practice && touch readme.md
echo "Hi there, this is a readme file." > readme.md
echo "This is the second line of the readme file." >> readme.md
mv readme.md readme.txt
mkdir document
mv readme.txt document/introduction.txt
cd document && cp introduction.txt readme.txt
echo "The quick brown fox jumps over a lazy dog" > readme.txt
cd .. && cp -r document docs
rm -r document
mkdir -p parent/child/docs
cp docs/introduction.txt parent/child/docs
```

