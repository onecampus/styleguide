# git commit 规范

1. 不用使用`-m` 和 `-a`, 直接 `git commit`， 然后在vim或其他编辑器
2. 第一行应该少于50个字。 随后是一个空行 第一行题目也可以写成: `Fix issue #8976`

```
Redirect user to the requested page after login

https://trello.com/path/to/relevant/card

Users were being redirected to the home page after login, which is less
useful than redirecting to the page they had originally requested before
being redirected to the login form.

* Store requested path in a session variable
* Redirect to the stored location after successfully logging in the user
```

```
Fix bug where user can't signup.

[Bug #2873942]

Users were unable to register if they hadn't visited the plans
and pricing page because we expected that tracking
information to exist for the logs we create after a user
signs up.  I fixed this by adding a check to the logger
to ensure that if that information was not available
we weren't trying to write it.
```

### 注释要回答如下信息

#### 为什么这次修改是必要的
#### 如何解决的问题
#### 这些变化可能影响哪些地方

### 小提示
* 使用 fix, add, change 而不是 fixed, added, changed

### 其他公司
* [jquery](http://contribute.jquery.org/commits-and-pull-requests/)
