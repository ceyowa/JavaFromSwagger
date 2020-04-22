# [动作](https://www.jetbrains.org/intellij/sdk/docs/basics/action_system.html)
Intellij提供的一个概念，就是一个继承自[_`AnAction`_](https://upsource.jetbrains.com/idea-ce/file/idea-ce-9276f4bbfb20dac51cdc0d675aef80b7f639a378/platform/editor-ui-api/src/com/intellij/openapi/actionSystem/AnAction.java) 的类，当点击选择菜单或对应的按钮，
则执行类的`actionPerformed()`方法.  
* 需要在plugin.xml文件里的`<actions>`节点添加  
* 支持直接添加`<action>`节点  
* 分组时添加至`<group>`节点  
* 支持从菜单和工具栏执行动作
* 支持添加快捷键，和`Find Action`(Ctrl + Shift + A)执行
* 支持动态添加动作，需要使用[_`ActionGroup`_]()
