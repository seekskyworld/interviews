# 序列化与反序列化

前端->发送JSON->

后端->接受JSON->

JSON转换为字典->

字典经过序列化转换成模型对象（调用create的某某模型.objects.create(**validated_data)）->

模型对象经过orm，存入数据库(当前序列化对象进行.save()，根据键值对生成sql语句，数据库进行运行)

![Snipaste_2024-06-04_09-22-57](./md图片/DRF/Snipaste_2024-06-04_09-22-57.png)



使用sql语句查询到值，从数据库取出模型对象，进行相关过滤操作->

模型对象经过反序列化转换成字典->

字典转换成JSON->

后端->发送JSON->

前端->接受JSON->

JSON就是相关数据

# 常用类概略图

![ModelSerializer](./md图片/DRF/ModelSerializer.jpg)

<img src="./md图片/DRF/ModelViewSet.jpg" alt="ModelViewSet"  />



# 日常使用技巧







# 第一天



![第1天](./md图片/DRF/第1天.png)

![第1天-1-序列化器默认不能对查询结果集进行转换](./md图片/DRF/第1天-1-序列化器默认不能对查询结果集进行转换.png)

![第1天-2-primarykey](./md图片/DRF/第1天-2-primarykey.png)

![第1天-3-外键](./md图片/DRF/第1天-3-外键.png)





# 第二天



![第2天](./md图片/DRF/第2天.png)

![第2天-1-data关键字不能省略](./md图片/DRF/第2天-1-data关键字不能省略.png)

![第2天-2-必须实现create方法](./md图片/DRF/第2天-2-必须实现create方法.png)

![第2天-3-序列化器的创建](./md图片/DRF/第2天-3-序列化器的创建.png)

![第2天-4-必须实现update方法](./md图片/DRF/第2天-4-必须实现update方法.png)

![第2天-5-重写字段属性](./md图片/DRF/第2天-5-重写字段属性.png)

![第2天-6-在序列化器中定义的字段一定要添加到fields中](./md图片/DRF/第2天-6-在序列化器中定义的字段一定要添加到fields中.png)

![第2天-7-序列化器嵌套序列化实现字典嵌套字典数据保存](./md图片/DRF/第2天-7-序列化器嵌套序列化实现字典嵌套字典数据保存.png)



# 第三天



![第3天-](./md图片/DRF/第3天-.png)

![第3天-0-GenericAPIVew通常要设置queryset和serializer_class](./md图片/DRF/第3天-0-GenericAPIVew通常要设置queryset和serializer_class.png)

![第3天-1-ListModelMixin](./md图片/DRF/第3天-1-ListModelMixin.png)

![第3天-2-CreaetModelMixin](./md图片/DRF/第3天-2-CreaetModelMixin.png)

![第3天-3-GenericAPIView与mixin配合使用的优势](./md图片/DRF/第3天-3-GenericAPIView与mixin配合使用的优势.png)

![第3天-4-get_object的源码解析](./md图片/DRF/第3天-4-get_object的源码解析.png)

![第3天-5-lookup_field](./md图片/DRF/第3天-5-lookup_field.png)

![第3天-6-RetrieveModelMixin](./md图片/DRF/第3天-6-RetrieveModelMixin.png)

![第3天-7-UpdateModelMixin](./md图片/DRF/第3天-7-UpdateModelMixin.png)

![第3天-8-DestoryModelMixin](./md图片/DRF/第3天-8-DestoryModelMixin.png)

![第3天-9-类的继承关系](./md图片/DRF/第3天-9-类的继承关系.png)

![第3天-10-分页类为什么不能分页](./md图片/DRF/第3天-10-分页类为什么不能分页.png)

![第3天-11-分页类为什么不能设置一页多少条记录](./md图片/DRF/第3天-11-分页类为什么不能设置一页多少条记录.png)

