This article explains how to load the online images in [.NET MAUI AvatarView](https://www.syncfusion.com/maui-controls/maui-avatarview). To display an online image in the AvatarView, it is recommended to set the [ContentType](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.Core.SfAvatarView.html?tabs=tabid-1#Syncfusion_Maui_Core_SfAvatarView_ContentType) property to [Custom](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.Core.ContentType.html#Syncfusion_Maui_Core_ContentType_Custom). This allows for the use of custom images, including those sourced from the web.

```xml
<VerticalStackLayout
    Padding="30,0"
    Spacing="25">
    <core:SfAvatarView AvatarSize="ExtraLarge"
                       HeightRequest="200"
                       AvatarShape="Square"
                       ContentType="Custom"
                       Aspect="AspectFill">
        <core:SfAvatarView.ImageSource>
            <UriImageSource Uri="https://cdn.syncfusion.com/content/images/Images/Camtasia_Succinctly.png?v=22022017060923"/>
        </core:SfAvatarView.ImageSource>
    </core:SfAvatarView>
</VerticalStackLayout>
```

- **ContentType**: Setting this property to `Custom` enables AvatarView to accept custom images.
- **ImageSource**: The `UriImageSource` is used to specify the URL of the image that you want to display.

By following this approach, you can easily load and display online images in your .NET MAUI applications.

**Output**

![AvatarView.png](https://support.syncfusion.com/kb/agent/attachment/article/17110/inline?token=eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjI4MTc2Iiwib3JnaWQiOiIzIiwiaXNzIjoic3VwcG9ydC5zeW5jZnVzaW9uLmNvbSJ9.enFMRhQ00OpCzZKqhwISFd5Q_D8bweCtCL435dUyNsI)