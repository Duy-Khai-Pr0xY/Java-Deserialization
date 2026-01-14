# Java-Deserialization
#### Java là một ngôn ngữ hướng đối tượng (object)
#### Java những cái khi mà muốn (lưu file, lưu dữ liệu vào db,gửu qua mạng......) thì thằng java nó sẽ serialize. Ngược lại nếu nó nhận dữ liệu trên mạng thì nó sẽ deserialize ra tái tạo lại cái object 
#### Hàm serialize trong java: writeObject
#### Hàm unserialize trong java: readObject
#### Chữ ký đầu tệp của java (file singnature 4 bytes) AC ED 00 05 (nhìn thấy 4 số này khả năng là serialize của java)
#### Classname: com.example.javaserialize.User..... và tên thuộc tinh và kiểu dữ liệu của thuộc tính đó và giá trị của thuộc tính 
#### Serial Version UID: mỗi class trong java sẽ có version uid khác nhau. Khi mà deserialize java sẽ kiểm tra version trong serialize_data và version của class đang có trên server để đảm bảo sự tương thích
# Magic methods trong Java
#### ClassName() (Khởi tạo), finalize() (Hủy obj), toString() (ép kiểu)
# Đặc biệt: tùy chỉnh được quá trình serialize và unserialize 
#### Làm sao để tùy chỉnh ??? => dev sẽ viết lại 2 method writeObject và readObject của chính 
# Root cause của lỗi Deserialize là untrusted_data quá trình unserialize (readObject)
#### Thay vì ngồi tự chỉnh nhờ java serialize cái payload 
#### Java muốn thay đổi dữ liệu thì cần phải build lại docker exec -it java_deserialize /home/cbjs/build.sh
