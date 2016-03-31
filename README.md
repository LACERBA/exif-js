#Exif.js

A JavaScript library for reading EXIF meta data from JPEG image files.


Exif.js 读取图像的元数据来源
Exif.js 提供了 JavaScript 读取图像的原始数据的功能扩展，例如：拍照方向、相机设备型号、拍摄时间、ISO 感光度、GPS 地理位置等数据。
注意事项：
EXIF 数据主要来自拍摄的照片，多用于移动端开发，PC 端也会用到，此插件兼容主流浏览器，IE10 以下不支持。
查看 Demo
下载 Exif.js
提交问题 / Bug / 建议

文档目录
使用方法API 方法EXIF 标识相关信息
使用方法
载入 JavaScript 文件
<script src="exif.js"></script>
获取 EXIF 数据
EXIF.getData(document.getElementById('imgElement'), function(){ 
  EXIF.getAllTags(this); 
  EXIF.getTag(this, 'Orientation'); 
}); 
API 方法
名称	说明
EXIF.getData(img, callback)	
获取图像的数据
能兼容尚未支持提供 EXIF 数据的浏览器获取到元数据。
EXIF.getTag(img, tag)	获取图像的某个数据
EXIF.getAllTags(img)	获取图像的全部数据，值以对象的方式返回
EXIF.pretty(img)	获取图像的全部数据，值以字符串的方式返回
EXIF 标识
名称	说明
ExifVersion	Exif 版本
FlashPixVersion	FlashPix 版本
ColorSpace	色域、色彩空间
PixelXDimension	图像的有效宽度
PixelYDimension	图像的有效高度
ComponentsConfiguration	图像构造
CompressedBitsPerPixel	压缩时每像素色彩位
MakerNote	制造商设置的信息
UserComment	用户评论
RelatedSoundFile	关联的声音文件
DateTimeOriginal	创建时间
DateTimeDigitized	数字化创建时间
SubsecTime	日期时间（秒）
SubsecTimeOriginal	原始日期时间（秒）
SubsecTimeDigitized	原始日期时间数字化（秒）
ExposureTime	曝光时间
FNumber	光圈值
ExposureProgram	曝光程序
SpectralSensitivity	光谱灵敏度
ISOSpeedRatings	感光度
OECF	光电转换功能
ShutterSpeedValue	快门速度
ApertureValue	镜头光圈
BrightnessValue	亮度
ExposureBiasValue	曝光补偿
MaxApertureValue	最大光圈
SubjectDistance	物距
MeteringMode	测光方式
Lightsource	光源
Flash	闪光灯
SubjectArea	主体区域
FocalLength	焦距
FlashEnergy	闪光灯强度
SpatialFrequencyResponse	空间频率反应
FocalPlaneXResolution	焦距平面X轴解析度
FocalPlaneYResolution	焦距平面Y轴解析度
FocalPlaneResolutionUnit	焦距平面解析度单位
SubjectLocation	主体位置
ExposureIndex	曝光指数
SensingMethod	图像传感器类型
FileSource	源文件
SceneType	场景类型（1 == 直接拍摄）
CFAPattern	CFA 模式
CustomRendered	自定义图像处理
ExposureMode	曝光模式
WhiteBalance	白平衡（1 == 自动，2 == 手动）
DigitalZoomRation	数字变焦
FocalLengthIn35mmFilm	35毫米胶片焦距
SceneCaptureType	场景拍摄类型
GainControl	场景控制
Contrast	对比度
Saturation	饱和度
Sharpness	锐度
DeviceSettingDescription	设备设定描述
SubjectDistanceRange	主体距离范围
InteroperabilityIFDPointer	
ImageUniqueID	图像唯一ID
Tiff 相关
名称	说明
ImageWidth	图像宽度
ImageHeight	图像高度
BitsPerSample	比特采样率
Compression	压缩方法
PhotometricInterpretation	像素合成
Orientation	拍摄方向
SamplesPerPixel	像素数
PlanarConfiguration	数据排列
YCbCrSubSampling	色相抽样比率
YCbCrPositioning	色相配置
XResolution	X方向分辨率
YResolution	Y方向分辨率
ResolutionUnit	分辨率单位
StripOffsets	图像资料位置
RowsPerStrip	每带行数
StripByteCounts	每压缩带比特数
JPEGInterchangeFormat	JPEG SOI 偏移量
JPEGInterchangeFormatLength	JPEG 比特数
TransferFunction	转移功能
WhitePoint	白点色度
PrimaryChromaticities	主要色度
YCbCrCoefficients	颜色空间转换矩阵系数
ReferenceBlackWhite	黑白参照值
DateTime	日期和时间
ImageDescription	图像描述、来源
Make	生产者
Model	型号
Software	软件
Artist	作者
Copyright	版权信息
GPS 相关
名称	说明
GPSVersionID	GPS 版本
GPSLatitudeRef	南北纬
GPSLatitude	纬度
GPSLongitudeRef	东西经
GPSLongitude	经度
GPSAltitudeRef	海拔参照值
GPSAltitude	海拔
GPSTimeStamp	GPS 时间戳
GPSSatellites	测量的卫星
GPSStatus	接收器状态
GPSMeasureMode	测量模式
GPSDOP	测量精度
GPSSpeedRef	速度单位
GPSSpeed	GPS 接收器速度
GPSTrackRef	移动方位参照
GPSTrack	移动方位
GPSImgDirectionRef	图像方位参照
GPSImgDirection	图像方位
GPSMapDatum	地理测量资料
GPSDestLatitudeRef	目标纬度参照
GPSDestLatitude	目标纬度
GPSDestLongitudeRef	目标经度参照
GPSDestLongitude	目标经度
GPSDestBearingRef	目标方位参照
GPSDestBearing	目标方位
GPSDestDistanceRef	目标距离参照
GPSDestDistance	目标距离
GPSProcessingMethod	GPS 处理方法名
GPSAreaInformation	GPS 区功能变数名
GPSDateStamp	GPS 日期
GPSDifferential	GPS 修正
相关信息
作者网站：https://github.com/jseidelin/exif-js
相关文档：Github中文文档

