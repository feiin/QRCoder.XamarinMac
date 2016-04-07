# QRCoder.XamarinMac
QRCodeGenerator,use CoreGraphics in Xamarin.Mac.


##using

```
.....
var qrGenerator = new QRCoder.QRCodeGenerator ();
var QrCodeView = new NSImageView (new CoreGraphics.CGRect(0, 0, 150, 150));
var qrCode = qrGenerator.CreateQrCode("http://www.baidu.com/", QRCoder.QRCodeGenerator.ECCLevel.M);
var qrImage = qrCode.GetGraphic(20);
QrCodeView.Image = qrImage;
......
```