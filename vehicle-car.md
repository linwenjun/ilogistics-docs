### 车辆相关

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
### 车辆参数相关
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
```

