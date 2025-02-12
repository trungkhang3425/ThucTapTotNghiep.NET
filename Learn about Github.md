# Tìm hiểu về GitHub

## Giới thiệu về GitHub
GitHub là nền tảng kiểm soát phiên bản và cộng tác, cho phép nhiều người cùng làm việc trên các dự án. Nền tảng này sử dụng Git, một hệ thống kiểm soát phiên bản phân tán, để theo dõi các thay đổi và quản lý cơ sở mã. GitHub cung cấp cả kho lưu trữ riêng tư và công khai, đồng thời cung cấp một số công cụ để tạo điều kiện cho cộng tác, đánh giá mã và tích hợp liên tục.

## Các khái niệm chính:
- **Kho lưu trữ (Repo)**: Không gian lưu trữ cho dự án của bạn, có thể là công khai hoặc riêng tư. Kho lưu trữ này chứa tất cả các tệp dự án của bạn, bao gồm mã, tài liệu, v.v.
- **Cam kết**: Ảnh chụp nhanh các thay đổi của bạn mà bạn có thể đẩy lên kho lưu trữ. Mỗi cam kết có một ID duy nhất và theo dõi các thay đổi đối với các tệp.
- **Nhánh**: Phiên bản song song của kho lưu trữ của bạn. Bạn có thể tạo nhánh để làm việc trên một tính năng hoặc sửa lỗi mà không ảnh hưởng đến cơ sở mã chính.
- **Yêu cầu kéo (PR)**: Một cách để yêu cầu hợp nhất mã từ nhánh này sang nhánh khác. Cách này thường được sử dụng để hợp nhất các nhánh tính năng vào nhánh chính sau khi đánh giá.
- **Fork**: Tạo bản sao của kho lưu trữ khác trong tài khoản GitHub của bạn. Điều này hữu ích khi bạn muốn đóng góp cho một dự án nguồn mở.

---

# Tìm hiểu về các hoạt động của GitHub với Azure trên Visual Studio

## Thiết lập GitHub với Azure trong Visual Studio
Visual Studio giúp bạn dễ dàng tích hợp GitHub với các dự án Azure của mình. Bằng cách kết nối GitHub với Visual Studio, bạn có thể quản lý kho lưu trữ, cộng tác trên mã và triển khai trực tiếp lên Azure.

### Các bước:
1. **Sao chép Kho lưu trữ GitHub**:
- Trong Visual Studio, hãy đi tới **Tệp > Mở > Mở từ Kiểm soát nguồn**.
- Chọn **GitHub** và nhập URL kho lưu trữ của bạn.
- Sau khi sao chép, bạn có thể bắt đầu sửa đổi mã của mình trong Visual Studio.

2. **Cam kết thay đổi**:
- Sử dụng cửa sổ **Thay đổi Git** để xem các tệp đã sửa đổi.
- Sau khi chỉnh sửa, hãy viết tin nhắn cam kết và nhấp vào **Cam kết tất cả** để lưu các thay đổi cục bộ.
- Đẩy các thay đổi của bạn lên GitHub bằng cách chọn **Đồng bộ hóa**.

3. **Triển khai lên Azure**:
- Bạn có thể triển khai ứng dụng trực tiếp từ Visual Studio lên Azure.
- Nhấp chuột phải vào dự án trong Solution Explorer, chọn **Publish** và chọn **Azure**.
- Làm theo lời nhắc để thiết lập tài khoản Azure của bạn và triển khai dự án.

---

# Tìm hiểu về các hoạt động GitHub với Azure trên Dòng lệnh

## Tích hợp GitHub và Azure CLI
Các hoạt động GitHub cũng có thể được quản lý bằng dòng lệnh, đặc biệt là với Giao diện dòng lệnh Azure (CLI). Azure CLI cho phép bạn tương tác với các tài nguyên Azure của mình trực tiếp từ thiết bị đầu cuối.

### Các bước:
1. **Cài đặt Git và Azure CLI**:
- Cài đặt Git để quản lý kho lưu trữ của bạn.
- Cài đặt Azure CLI để tương tác với các tài nguyên Azure của bạn.

2. **Sao chép Kho lưu trữ GitHub**:
- Sử dụng lệnh sau để sao chép kho lưu trữ:
```bash
git clone https://github.com/username/repository.git

3. **Commit and Push Changes**: 
- Sau khi thực hiện thay đổi cục bộ:

````bash
git add .
git commit -m "Your commit message"
git push origin main

4. **Deploy to Azure**:
- Use the Azure CLI to deploy your project:

az webapp up --name YourAppName --resource-group YourResourceGroup


### **Commit Changes**
- Sau khi bạn đã thêm nội dung vào tệp `.md`, kéo xuống dưới và nhấn **Commit new file**.
- Bạn có thể nhập một thông điệp commit như: "Add Learn about GitHub and Azure operations document".

### **Xem Kết Quả**
- Sau khi commit, bạn có thể mở tệp `.md` trong kho chứa của mình trên GitHub để xem kết quả.

GitHub sẽ tự động render nội dung Markdown thành văn bản có định dạng đẹp mắt, bao gồm các tiêu đề, danh sách, mã code, và các đoạn văn bản đã được định dạng.

Hãy thử làm theo các bước này và xem kết quả!
