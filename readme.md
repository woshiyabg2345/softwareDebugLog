# 软件调试记录

1.调试遇到vector 变量在clear 时程序崩溃，vector 中存放的是自定义的结构体，而且提示结构体中的string 类型在析构时出现错误，最后发现在程序中定义了相同的结构体名称，虽然使用了typedef 但是内存中仍然使用的是struct 之后的名称。
