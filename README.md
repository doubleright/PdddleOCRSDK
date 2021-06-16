# PdddleOCRSDK



```c#
    
    /// <summary>
    /// 识别单行纯净的文本图片
    /// </summary>
    /// <param name="input"></param>
    /// <param name="height"></param>
    /// <param name="width"></param>
    /// <returns></returns>
    [DllImport("BarcodeSDK.dll", EntryPoint = "ReadLine", SetLastError = true, CharSet = CharSet.Unicode)]
    public static extern IntPtr ReadLine(byte[] input, int height, int width);  //out string
        
    /// <summary>
    /// 识别整个图片所有文本框检测的内容
    /// </summary>
    /// <param name="input"></param>
    /// <param name="height"></param>
    /// <param name="width"></param>
    /// <returns></returns>
    [DllImport("BarcodeSDK.dll", EntryPoint = "ReadAll", SetLastError = true, CharSet = CharSet.Unicode)]
    public static extern IntPtr ReadAll(byte[] input, int height, int width);  //out string

    /// <summary>
    /// 加载配置文件
    /// </summary>
    /// <param name="filepath"></param>
    [DllImport("BarcodeSDK.dll", EntryPoint = "LoadConfig", SetLastError = true, CharSet = CharSet.Unicode)]
    public static extern void LoadConfig(byte[] filepath);  //out void
```



飞浆预测SDK实现，c#也可以调用

![image-20210616142046172](D:\doubleright\PdddleOCRSDK\imgs\image-20210616142046172.png)

这速度还算满意？![image-20210616142239670](D:\doubleright\PdddleOCRSDK\imgs\image-20210616142239670.png)