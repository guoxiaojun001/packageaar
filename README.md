# packageaar
关于打包aar出现 错误: 需要常量表达式，的问题


Error:(149, 22) 错误: 需要常量表达式

解决方式： 将 switch中的case 改成 if 判断就可以了；注意：一般都会有提示的直接Alt+Enter就可以了； 
如果没有提示并且还缺少.R 文件的提示的话； 
解决方式：单独生成一下依赖包：Build–> Make Module “XXX” ; XXX: 对应的依赖包；这样就会有提示并解决问题了；


此问题可能是4.0之后变更的原因导致的，导致R文件找不到，具体原因不是很清楚，反正大家以后在用switch时候，如果考虑到后续需要打包
那么最好写成if else形式
