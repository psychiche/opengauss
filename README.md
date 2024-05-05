# GORM OpenGauss Driver

## Quick Start

```go
import (
  "gorm.io/driver/opengauss"
  "gorm.io/gorm"
)

dsn := "host=localhost user=gorm password=gorm dbname=gorm port=9920 sslmode=disable TimeZone=Asia/Shanghai"
db, err := gorm.Open(opengauss.Open(dsn), &gorm.Config{})
```

## Configuration

```go
import (
  "gorm.io/driver/postgres"
  "gorm.io/gorm"
)

db, err := gorm.Open(postgres.New(postgres.Config{
  DSN: "host=localhost user=gorm password=gorm dbname=gorm port=9920 sslmode=disable TimeZone=Asia/Shanghai", // data source name
}), &gorm.Config{})
```


Checkout [https://gorm.io](https://gorm.io) for details.
