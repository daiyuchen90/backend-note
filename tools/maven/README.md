####    指令
-   mvn clean -pl com.canopus.website:webapp-backend -am         对指定模块及其依赖模块打包
-   或者  mvn clean compile -U -pl webapp-backend -am                    
~~~test
参数	全称	释义	说明
-pl	--projects	Build specified reactor projects instead of all projects	
选项后可跟随{groupId}:{artifactId}或者所选模块的相对路径(多个模块以逗号分隔)

-am	--also-make	If project list is specified, also build projects required by the list	
表示同时处理选定模块所依赖的模块

-amd	--also-make-dependents	If project list is specified, also build projects that depend on projects on the list	
表示同时处理依赖选定模块的模块

-N	--Non-recursive	Build projects without recursive	
表示不递归子模块

-rf	--resume-from	Resume reactor from specified project	
表示从指定模块开始继续处理

~~~