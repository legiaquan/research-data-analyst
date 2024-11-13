# AWS Glue

![AWS Glue](assets/images/aws-glue.png)

## Tổng quan
AWS Glue là một dịch vụ ETL (trích xuất, chuyển đổi và tải) được quản lý hoàn toàn, giúp dễ dàng chuẩn bị và tải dữ liệu cho phân tích. Nó tự động khám phá và lập hồ sơ dữ liệu của bạn, đề xuất và tạo mã ETL, đồng thời xử lý tất cả cơ sở hạ tầng cơ bản.

## Tính năng chính
- **Serverless**: Không cần quản lý cơ sở hạ tầng, tự động cung cấp tài nguyên khi cần
- **Data Catalog**: Kho lưu trữ metadata trung tâm tự động khám phá và lập danh mục tài sản dữ liệu
- **Lập lịch công việc**: Trình lập lịch tích hợp để chạy các công việc ETL định kỳ
- **Điểm phát triển**: Môi trường phát triển tương tác để phát triển script ETL
- **Dynamic Frame**: Cấu trúc dữ liệu phân tán được tối ưu hóa cho các hoạt động ETL

## Thành phần
### Data Catalog
- **Tự động khám phá lược đồ**: Tự động suy luận lược đồ từ dữ liệu nguồn
- **Quản lý phiên bản**: Theo dõi thay đổi đối với định nghĩa bảng và lược đồ
- **Tích hợp**: Hoạt động liền mạch với các dịch vụ AWS khác như Athena, Redshift và EMR

### ETL Engine
- **Xây dựng trên Apache Spark**: Tận dụng khả năng xử lý phân tán
- **Nhiều ngôn ngữ**: Hỗ trợ Python và Scala để phát triển script ETL
- **Chuyển đổi tích hợp**: Cung cấp các thao tác chuyển đổi thông thường
- **Chuyển đổi tùy chỉnh**: Khả năng viết logic chuyển đổi tùy chỉnh

## Trường hợp sử dụng
- **ETL Data Lake**: Chuyển đổi và chuẩn bị dữ liệu để phân tích trong data lakes
- **Tải Data Warehouse**: Tải hiệu quả dữ liệu vào kho dữ liệu như Redshift
- **Xử lý Log**: Xử lý và phân tích log ứng dụng và hệ thống
- **ETL thời gian thực**: Hỗ trợ ETL luồng với Glue Studio

## Thực tiễn tốt nhất
- **Đánh dấu**: Sử dụng đánh dấu công việc để xử lý dữ liệu mới theo cách tăng dần
- **Giám sát**: Thiết lập giám sát CloudWatch cho số liệu công việc
- **Bảo mật**: Triển khai vai trò IAM và mã hóa phù hợp
- **Tối ưu chi phí**: Sử dụng loại worker và năng lực phù hợp với khối lượng công việc

## Tích hợp với các dịch vụ khác
- **Amazon S3**: Nguồn và đích cho xử lý dữ liệu
- **Amazon Redshift**: Tải dữ liệu đã chuyển đổi vào kho dữ liệu
- **Amazon Athena**: Truy vấn dữ liệu sử dụng Glue Data Catalog
- **Amazon EMR**: Chạy công việc Spark với Glue Data Catalog

## Kết luận
AWS Glue cung cấp giải pháp toàn diện cho nhu cầu ETL trong kiến trúc dữ liệu hiện đại, giúp dễ dàng chuẩn bị và chuyển đổi dữ liệu cho phân tích trong khi giảm thiểu chi phí vận hành.