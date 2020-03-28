# typedef声明
您可以使用 typedef 为一个已有的类型取一个新的名字。下面是使用 typedef 定义一个新类型的语法：

    typedef type newname; 
例如，下面的语句会告诉编译器，feet 是 int 的另一个名称：

    typedef int feet;
现在，下面的声明是完全合法的，它创建了一个整型变量 distance：

    feet distance;
#枚举类型
枚举类型声明一个可选的类型名称和一组标识符，用来作为该类型的值。其带有零个或多个标识符可以被用来作为该类型的值。每个枚举数是一个枚举类型的常数。

创建枚举，需要使用关键字 enum。枚举类型的一般形式为：

    enum enum-name { list of names } var-list; 
在这里，enum-name 是枚举类型的名称。名称列表 { list of names } 是用逗号分隔的。

例如，下面的代码定义了一个颜色枚举，变量 c 的类型为 color。最后，c 被赋值为 "blue"。

    enum color { red, green, blue } c;
    c = blue;
默认情况下，第一个名称的值为 0，第二个名称的值为 1，第三个名称的值为 2，以此类推。但是，您也可以给名称赋予一个特殊的值，只需要添加一个初始值即可。例如，在下面的枚举中，green 的值为 5。

    enum color { red, green=5, blue };
在这里，blue 的值为 6，因为默认情况下，每个名称都会比它前面一个名称大 1。
