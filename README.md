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
