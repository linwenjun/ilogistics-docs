### 车辆属性对象

```json

vendorId: Number
vendorName: String
cityId: Number
cityName: String
licensePlate: String
operationQualification: String //运营资质
brand: String
energyType: String
loadNumber: Number
licensedDate: Date
rating
techLevel
hasCamera
hasGps
seatInsuranceAmount： 座位险额度
maintainPeriod 保养周期
driverId
driverName
status：状态，1有效/0无效
operationCertificate: 营运证
drivingLicense
otherAttachments


# 查询中的年限
licensedYearUpperBound
licensedYearLowerBound
```



### 车辆相关接口和relation

```
# 获取车辆列表
relation vehicle-search-cars
GET vehicle/cars

# 获取单个车辆详情
relation vehicle-get-car-by-id
GET vehicle/cars/{id}

# 新增车辆
relation vehicle-create-car
POST vehicle/cars

# 修改车辆
relation vehicle-update-car
PUT vehicle/cars

# 删除车辆
relation vehicle-delete-car
DELETE vehicle/cars{id}
```
### 车辆参数相关接口和relation
```
# 获取 <类型> 列表
relation vehicle-get-car-energy-types
GET vehicle/cars/energy-types

# 获取 <等级评定> 列表
relation vehicle-search-car-ratings
GET vehicle/cars/ratings

# 获取 <技术等级> 列表
relation vehicle-search-car-tech-levels
GET vehicle/cars/tech-levels

# 获取 <运营资质> 列表
relation vehicle-search-car-operation-qualification
GET vehicle/cars/operation-qualifications

# 获取 <司机列表> 
relation vehicle-search-driver-by-vendor-id
GET vehicle/vendor/{id}/drivers
```