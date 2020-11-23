# commitlint-demo
使用commitlint以[conventional规范](https://www.conventionalcommits.org/)来约束commit message

## Usage

```
$ git add .
$ git commit -m "foo"
husky > commit-msg (node v12.7.0)
⧗   input: foo
✖   subject may not be empty [subject-empty]
✖   type may not be empty [type-empty]

✖   found 2 problems, 0 warnings
ⓘ   Get help: https://github.com/conventional-changelog/commitlint/#what-is-commitlint

husky > commit-msg hook failed (add --no-verify to bypass)
error Command failed with exit code 1.

$ git commit -m "chore: setup"
husky > commit-msg (node v12.7.0)
[master 78d2ecf] chore: setup
 1 file changed, 14 insertions(+)
 create mode 100644 README.md
```
### use prompt
```
$ git add .
$ yarn commit
yarn run v1.17.3
$ commit


Please enter a type: [required] [tab-completion] [header]
<type> holds information about the goal of a change.



<type>(<scope>): <subject>
<body>
<footer>


100 characters left
❯ type:
```

## 参考
https://medium.com/@klauskpm/how-to-create-good-commit-messages-67943d30cced

https://commitlint.js.org/#/guides-use-prompt