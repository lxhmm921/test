# test
cropper插件
插件地址：http://www.htmleaf.com/jQuery/Image-Effects/201504211716.html
配置参数
你可以通过$().cropper(options)方法来设置参数。如果你想改变全局默认参数，可以使用$.fn.cropper.setDefaults(options)方法。

aspectRatio：类型：Number，默认值NaN。设置剪裁容器的比例。
crop：类型：Function，默认值null。当改变剪裁容器或图片时的事件函数。
preview：类型：String(jQuery选择器)，默认值''。添加额外的元素（容器）的预览。注意：
最大宽度是剪裁容器的初始化宽度
最大高度是剪裁容器的初始化高度
如果你设置了aspectRatio参数，确保预览容器具有相同的比例
strict：类型：Boolean，默认值true。在strict模式中，canvas不能小于容器，剪裁容器不能再canvas之外。
responsive：类型：Boolean，默认值true。是否在窗口尺寸改变的时候重置cropper。
checkImageOrigin：类型：Boolean，默认值true。默认情况下，插件会检测图片的源，如果是跨域图片，图片元素会被添加crossOrigin class，并会为图片的url添加一个时间戳来使getCroppedCanvas变为可用。添加时间戳会使图片重新加载，以使跨域图片能够使用getCroppedCanvas。在图片上添加crossOrigin class会阻止在图片url上添加时间戳，及图片的重新加载。
background：类型：Boolean，默认值true。是否在容器上显示网格背景。
modal：类型：Boolean，默认值true。是否在剪裁框上显示黑色的模态窗口。
guides：类型：Boolean，默认值true。是否在剪裁框上显示虚线。
highlight：类型：Boolean，默认值true。是否在剪裁框上显示白色的模态窗口。
autoCrop：类型：Boolean，默认值true。是否在初始化时允许自动剪裁图片。
autoCropArea：类型：Number，默认值0.8（图片的80%）。0-1之间的数值，定义自动剪裁区域的大小。
dragCrop：类型：Boolean，默认值true。是否允许移除当前的剪裁框，并通过拖动来新建一个剪裁框区域。
movable：类型：Boolean，默认值true。是否允许移动剪裁框。
resizable：类型：Boolean，默认值true。是否允许改变剪裁框的大小。
zoomable：类型：Boolean，默认值true。是否允许放大缩小图片。
mouseWheelZoom：类型：Boolean，默认值true。是否允许通过鼠标滚轮来缩放图片。
touchDragZoom：类型：Boolean，默认值true。是否允许通过触摸移动来缩放图片。
rotatable：类型：Boolean，默认值true。是否允许旋转图片。
minContainerWidth：类型：Number，默认值200。容器的最小宽度。
minContainerHeight：类型：Number，默认值100。容器的最小高度。
minCanvasWidth：类型：Number，默认值0。canvas 的最小宽度（image wrapper）。
minCanvasHeight：类型：Number，默认值0。canvas 的最小高度（image wrapper）。
build：类型：Function，默认值null。build.cropper事件的简写方式。
built：类型：Function，默认值null。built.cropper事件的简写方式。
dragstart：类型：Function，默认值null。dragstart.cropper事件的简写方式。
dragmove：类型：Function，默认值null。dragmove.cropper事件的简写方式。
dragend：类型：Function，默认值null。dragend.cropper事件的简写方式。
zoomin：类型：Function，默认值null。zoomin.cropper事件的简写方式。
zoomout：类型：Function，默认值null。zoomout.cropper事件的简写方式。
