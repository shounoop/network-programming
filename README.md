# **I. JDBC --> pagekage (API) of java for connect java to database**

## **1. JDBC AP**

## **2. JDBC Driver Manager (gồm 4 loại): Quản lý Drivers để kết nối với database phù hợp**

1. Loại 1: JDBC-ODBC Bridge -> mất tích/k ai dùng nữa
2. Loại 2: Native-API, partly Java driver
3. Loại 3: JDBC-net, pure Java driver (gồm 3 tầng)

```
- Ứng dụng: JDBC client -> socket
- Middleware: Socket -> DBMS API (Loại 1, 2 hoặc 4)
- Database
```

4. Loại 4: Proprietary-Protocal Net (Phổ biến nhất hiện nay)

```
- Giao tiếp trực tiếp hệ CSDL không cần chuyển đổi thông qua socket
```
## **3. Bảy bước làm việc với JDBC**
1. Nạp driver
2. Định nghĩa Connection URL
3. Kết nối CSDL bằng đối tượng Connection
4. Tạo đối tượng Statement
5. Thi hành câu truy trấn
6. Xử lý kết quả
7. Đóng kết nối