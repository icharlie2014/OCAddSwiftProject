# OCAddSwiftProject
OC调用Swift代码


项目是OC的，但是需要使用到Swift
步骤：

1.将需要的swift文件拖到工程之后，新建头文件: 项目名-Bridging-Header.h

2.在Build Settings里搜索swift -> Objective-C Bridging Header

填上：$(PROJECT)/项目名-Bridging-Header.h

3.最后使用了，由于swift没有头文件，故导入#import "项目名-Swift.h"

之后就可以使用swift了。