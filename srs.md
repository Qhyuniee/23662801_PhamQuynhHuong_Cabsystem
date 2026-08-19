
# Bước 1: Xác định ngữ cảnh nghiệp vụ và vấn đề nghiệp vụ
Trả lời: khách hàng muốn giải quyết vấn đề gì, tại sao ko thể đáp ứng, ai sẽ là người sd hệ thống,mục tiêu kinh doanh,giá trị của hệ thống này tạo ra so với hệ thống cũ là gì

# Ngữ cảnh nghiệp vụ
Công ty ABC là doanh nghiệp cung cấp dịch vụ đặt xe trực tuyến. Hiện tại, khách hàng đặt xe thông qua tổng đài hoặc một ứng dụng đơn giản. Quy trình hoạt động liên quan đến khách hàng đặt xe, tìm và phân công tài xế, thực hiện chuyến đi, tính cước, thanh toán và quản lý hoạt động.
Do số lượng khách hàng và tài xế có nhu cầu tăng, công ty muốn xây dựng CAB System – nền tảng đặt xe mới có khả năng tự động hóa quy trình, phục vụ số lượng lớn người dùng và dễ dàng mở rộng trong tương lai.

# Vấn đề nghiệp vụ
Hệ thống hiện tại của công ty ABC đang gặp các vấn đề:
-Phân công tài xế chủ yếu thủ công, làm giảm hiệu quả xử lý yêu cầu đặt xe.
-Khách hàng khó theo dõi trạng thái chuyến đi, như đang tìm tài xế, tài xế đã nhận chuyến hay tài xế đã đến.
-Thông tin thanh toán chưa được quản lý tập trung, gây khó khăn trong quản lý và tra cứu giao dịch.
-Bộ phận vận hành gặp khó khăn trong quản lý khách hàng, tài xế, phương tiện và các chuyến đi.
-Hệ thống hiện tại khó đáp ứng khi số lượng khách hàng, tài xế và chuyến đi tăng cao.
-Khó mở rộng hoặc bổ sung chức năng mới như loại dịch vụ, phương thức thanh toán và kênh thông báo.


# B2.xác định stakeholder

# Lập bảng: cột 1: những stakeholder,cột 2: vai trò của stakeholder

| Stakeholder | Vai trò |
|---|---|
| Ban lãnh đạo | Đưa ra yêu cầu, mục tiêu kinh doanh và định hướng phát triển hệ thống |
| Khách hàng | Đặt xe, theo dõi chuyến đi, thanh toán và đánh giá tài xế |
| Tài xế | Nhận chuyến và thực hiện chuyến đi |
| Nhân viên vận hành/Admin | Quản lý và giám sát hoạt động của hệ thống |
| Nhà cung cấp dịch vụ bên ngoài | Hỗ trợ thanh toán điện tử và cung cấp dịch vụ gửi thông báo |

# Vẽ ma trận stakeholder(stakeholder matrix): để biết mức độ ảnh hưởng của các vai trò trong hệ thống
                         MỨC ĐỘ QUAN TÂM
                   THẤP                    CAO
             ┌──────────────────┬─────────────────────────┐
 Quyền lực   │ KEEP SATISFIED   │ MANAGE CLOSELY          │
    CAO      │                  │                         │
             │ Nhà cung cấp     │ • Ban lãnh đạo          │
             │ dịch vụ bên ngoài│ • NV vận hành/Admin     │
             ├──────────────────┼─────────────────────────┤
 Quyền lực   │ MONITOR          │ KEEP INFORMED           │
    THẤP     │                  │                         │
             │ • Không có       │ • Khách hàng            │
             │                  │ • Tài xế                │
             └──────────────────┴─────────────────────────┘
# B3: Mục đích nghiệp vụ: ko cố gắng biến mong muốn của khách hàng thành chức năng
business goal: đặt tên là BG, ví dụ BG01: tăng hiệu quả thanh toán
- hỗ trợ thanh toán bằng tiền mặt/ trực tuyến
  BG02: giảm thời gian tìm tài xế:
  cho phép tìm tài xế tự động

# Business Goal

BG01: Tăng hiệu quả phân công tài xế:
Cho phép tự động tìm và phân công tài xế phù hợp dựa trên vị trí và trạng thái sẵn sàng.

BG02: Giảm thời gian tìm tài xế:
Cho phép tự động tìm tài xế gần khách hàng và tiếp tục tìm tài xế khác khi tài xế được đề xuất từ chối hoặc không phản hồi.

BG03: Nâng cao trải nghiệm khách hàng:
Cho phép khách hàng theo dõi trạng thái chuyến đi và nhận thông báo trong quá trình đặt xe.

BG04: Quản lý thanh toán tập trung:
Cho phép tính cước, lưu thông tin giao dịch và hỗ trợ thanh toán bằng tiền mặt hoặc thanh toán điện tử.

BG05: Nâng cao hiệu quả vận hành:
Cho phép nhân viên quản lý và theo dõi khách hàng, tài xế, phương tiện, chuyến đi và giao dịch trên cùng hệ thống.

BG06: Hỗ trợ quản lý hoạt động kinh doanh:  
Cung cấp báo cáo về số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả hoạt động của tài xế.

BG07: Tăng khả năng mở rộng:
Cho phép hệ thống phục vụ số lượng lớn khách hàng và tài xế, đồng thời dễ dàng bổ sung dịch vụ và chức năng mới trong tương lai.

# B4: Xác định phạm vi(scope): bóp phạm vi lại

Trong phạm vi – In Scope
-Quản lý tài khoản: Cho phép khách hàng và tài xế đăng ký, đăng nhập và cập nhật thông tin cá nhân.
-Đặt xe: Cho phép khách hàng nhập điểm đón, điểm đến, lựa chọn loại xe và gửi yêu cầu đặt xe.
-Nhận chuyến: Cho phép tài xế nhận hoặc từ chối chuyến; nếu tài xế từ chối hoặc không phản hồi, hệ thống tiếp tục tìm tài xế khác.
-Theo dõi chuyến đi: Cho phép khách hàng theo dõi trạng thái chuyến và tài xế cập nhật trạng thái trong quá trình thực hiện.
-Quản lý vị trí tài xế: Lưu vị trí tài xế để hỗ trợ tìm tài xế gần khách hàng và dự kiến thời gian đến.
-Tính cước và thanh toán: Tính số tiền chuyến đi và hỗ trợ thanh toán bằng tiền mặt hoặc thanh toán điện tử.
-Thông báo: Gửi thông báo cho khách hàng và tài xế về các trạng thái quan trọng của chuyến đi và thanh toán.
-Lịch sử và đánh giá: Cho phép khách hàng xem lịch sử chuyến đi và đánh giá tài xế.
-Quản lý vận hành: Cho phép nhân viên vận hành/Admin quản lý khách hàng, tài xế, phương tiện, chuyến đi và giao dịch.
-Phân quyền và bảo mật: Xác thực người dùng, kiểm soát quyền truy cập và lưu vết các thao tác quan trọng.
-Báo cáo: Cung cấp báo cáo về số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế.

Ngoài phạm vi
-Chưa bổ sung các loại dịch vụ vận chuyển mới ngoài các loại dịch vụ được xác định trong phiên bản hiện tại.
-Chưa tích hợp nhiều nhà cung cấp thanh toán, chỉ tích hợp với nhà cung cấp thanh toán được lựa chọn trong giai đoạn hiện tại.
-Chưa bổ sung nhiều kênh hoặc nhà cung cấp thông báo mới, chỉ cần đảm bảo hệ thống có khả năng mở rộng trong tương lai.
-Không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán trong CAB System.


# b5Chuyển đổi thành các business requirement(BR): cột 1 là mã,cột 2 là tên, cột 3 diễn giải
ví dụ: 
BR01: Theo dõi chuyến đi:
Khách hàng có khả năng theo dõi chuyến đi trong suốt quá trình di chuyển

| Mã | Tên | Diễn giải |
|---|---|---|
| BR01 | Hỗ trợ quy trình đặt xe trực tuyến | Hỗ trợ khách hàng thực hiện quy trình đặt xe từ khi tạo yêu cầu đến khi hoàn thành chuyến đi. |
| BR02 | Tự động hóa tìm và phân công tài xế | Tự động tìm tài xế phù hợp dựa trên vị trí, trạng thái sẵn sàng và các tiêu chí vận hành. |
| BR03 | Đảm bảo khả năng tìm tài xế liên tục | Khi tài xế từ chối hoặc không phản hồi, tiếp tục tìm tài xế khác mà khách hàng không cần tạo lại yêu cầu. |
| BR04 | Hỗ trợ theo dõi chuyến đi | Cho phép khách hàng và nhân viên vận hành theo dõi trạng thái chuyến đi. |
| BR05 | Quản lý tài xế và phương tiện | Quản lý thông tin tài xế, phương tiện, trạng thái hoạt động và vị trí tài xế. |
| BR06 | Quản lý tính cước và thanh toán | Hỗ trợ tính cước và thanh toán bằng tiền mặt hoặc phương thức điện tử. |
| BR07 | Quản lý thông báo | Gửi thông báo cho khách hàng và tài xế về chuyến đi và kết quả thanh toán. |
| BR08 | Hỗ trợ quản lý và vận hành | Quản lý khách hàng, tài xế, phương tiện, chuyến đi, giao dịch và hỗ trợ xử lý sự cố. |
| BR09 | Hỗ trợ báo cáo kinh doanh | Cung cấp báo cáo số chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế. |
| BR10 | Đảm bảo bảo mật và phân quyền | Xác thực người dùng, kiểm soát quyền truy cập, bảo vệ dữ liệu và lưu vết thao tác quan trọng. |
| BR11 | Đảm bảo khả năng mở rộng và ổn định | Đáp ứng số lượng lớn người dùng và hạn chế lỗi của một chức năng ảnh hưởng toàn hệ thống. |
| BR12 | Hỗ trợ phát triển trong tương lai | Cho phép bổ sung dịch vụ, phương thức thanh toán và kênh thông báo mới trong tương lai. |

# B6: BUSINESS PROCESS( QUY TRÌNH NGHIỆP VỤ): sử dụng mermaid
VÍ DỤ: Khách hàng tạo chuyến đi- hệ thống xác nhận- tìm tài xế

# B7: Viết functional requirement(FR) (từ 1 cái yêu cầu thì phân rã ra) 
ví dụ: 
FR01: xác định vị trí khách
FR02: Tìm tài xế sẵn có
FR03: Lọc theo loại xe
FR04: Tính khoảng cách từ điểm đi đến điểm đón

Phân rã quản lý khách hàng:
đăng ký-đăng nhập-cập nhật thông tin-xem thông tin
# 1. Quản lý tài khoản
FR01: Đăng ký tài khoản khách hàng
FR02: Đăng ký tài khoản tài xế
FR03: Đăng nhập
FR04: Cập nhật thông tin cá nhân
FR05: Cập nhật hồ sơ tài xế
# 2. Đặt xe
FR06: Xác định vị trí khách hàng
FR07: Nhập điểm đón
FR08: Nhập điểm đến
FR09: Lựa chọn loại xe
FR10: Tính khoảng cách từ điểm đón đến điểm đến
FR11: Gửi yêu cầu đặt xe
# 3. Tìm và phân công tài xế
FR12: Tìm tài xế sẵn có
FR13: Lọc tài xế theo loại xe
FR14: Xác định vị trí tài xế
FR15: Tính khoảng cách từ tài xế đến điểm đón
FR16: Ưu tiên tài xế phù hợp và gần khách hàng
FR17: Gửi yêu cầu chuyến đến tài xế
# 4. Nhận chuyến
FR18: Chấp nhận chuyến
FR19: Từ chối chuyến
FR20: Kiểm tra thời gian phản hồi của tài xế
FR21: Tìm tài xế khác khi tài xế từ chối hoặc không phản hồi
FR22: Thông báo khi không tìm được tài xế
# 5. Theo dõi chuyến đi
FR23: Hiển thị thông tin tài xế nhận chuyến
FR24: Hiển thị thời gian dự kiến tài xế đến
FR25: Cập nhật trạng thái đã đến điểm đón
FR26: Cập nhật trạng thái đã đón khách
FR27: Cập nhật trạng thái đang di chuyển
FR28: Cập nhật trạng thái hoàn thành chuyến
FR29: Theo dõi trạng thái chuyến đi
# 6. Quản lý vị trí tài xế
FR30: Cập nhật vị trí tài xế
FR31: Lưu thông tin vị trí tài xế
FR32: Sử dụng vị trí để tìm tài xế gần khách hàng
FR33: Dự kiến thời gian tài xế đến điểm đón
# 7. Tính cước và thanh toán
FR34: Tính cước chuyến đi
FR35: Hiển thị số tiền phải trả
FR36: Thanh toán bằng tiền mặt
FR37: Thanh toán điện tử
FR38: Nhận kết quả thanh toán
FR39: Thông báo thanh toán thất bại
FR40: Thực hiện lại thanh toán
# 8. Thông báo
FR41: Thông báo yêu cầu đặt xe được tiếp nhận
FR42: Thông báo tài xế nhận chuyến
FR43: Thông báo tài xế đến điểm đón
FR44: Thông báo chuyến đi hoàn thành
FR45: Thông báo kết quả thanh toán
FR46: Thông báo chuyến mới cho tài xế
# 9. Lịch sử và đánh giá
FR47: Xem lịch sử chuyến đi
FR48: Xem chi tiết chuyến đi
FR49: Đánh giá tài xế sau chuyến đi
# 10. Quản lý vận hành
FR50: Quản lý khách hàng
FR51: Quản lý tài xế
FR52: Quản lý phương tiện
FR53: Quản lý chuyến đi
FR54: Theo dõi chuyến đang diễn ra
FR55: Kiểm tra trạng thái tài xế
FR56: Tra cứu lịch sử giao dịch
FR57: Hỗ trợ xử lý chuyến gặp lỗi
# 11. Phân quyền và bảo mật
FR58: Xác thực người dùng
FR59: Phân quyền nhân viên
FR60: Kiểm soát quyền truy cập
FR61: Lưu vết các thao tác quan trọng
# 12. Báo cáo
FR62: Báo cáo số lượng chuyến
FR63: Báo cáo doanh thu
FR64: Báo cáo tỷ lệ chuyến hoàn thành
FR65: Báo cáo tỷ lệ hủy chuyến
FR66: Báo cáo hiệu quả hoạt động tài xế
 # B8: quy tắc nghiệp vụ và ngoại lệ(business rule and exception)
 ví dụ exception: thanh toán thất bại
 ## Quy tắc nghiệp vụ và ngoại lệ

### 1. Quy tắc nghiệp vụ (Business Rules)

| Mã | Quy tắc nghiệp vụ | Diễn giải |
|---|---|---|
| BRU01 | Khách hàng phải đăng nhập trước khi đặt xe | Chỉ khách hàng đã được xác thực mới được gửi yêu cầu đặt xe. |
| BRU02 | Chuyến đi phải có điểm đón và điểm đến | Hệ thống chỉ tiếp nhận yêu cầu khi khách hàng cung cấp đầy đủ điểm đón và điểm đến. |
| BRU03 | Chỉ tài xế sẵn sàng mới được nhận chuyến | Tài xế phải ở trạng thái sẵn sàng và đáp ứng yêu cầu loại xe mới được hệ thống lựa chọn. |
| BRU04 | Ưu tiên tài xế phù hợp và gần khách hàng | Hệ thống lựa chọn tài xế dựa trên vị trí, trạng thái sẵn sàng và các tiêu chí vận hành. |
| BRU05 | Một chuyến chỉ được một tài xế nhận tại một thời điểm | Khi chuyến đã được một tài xế chấp nhận, hệ thống không phân công chuyến đó cho tài xế khác. |
| BRU06 | Tài xế phải phản hồi trong thời gian quy định | Nếu tài xế không phản hồi trong thời gian quy định, hệ thống xem là không nhận chuyến. |
| BRU07 | Tự động tìm tài xế khác | Nếu tài xế từ chối hoặc không phản hồi, hệ thống tiếp tục tìm tài xế khác mà khách hàng không cần đặt lại. |
| BRU08 | Trạng thái chuyến phải được cập nhật | Trạng thái chuyến được cập nhật trong suốt quá trình từ khi tài xế nhận chuyến đến khi hoàn thành. |
| BRU09 | Chỉ tính cước khi chuyến hoàn thành | Số tiền phải trả được xác định dựa trên loại dịch vụ và thông tin chuyến đi. |
| BRU10 | Thanh toán theo phương thức được hỗ trợ | Khách hàng có thể thanh toán bằng tiền mặt hoặc thanh toán điện tử. |
| BRU11 | Không lưu thông tin thanh toán nhạy cảm | Hệ thống CAB không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán. |
| BRU12 | Chỉ đánh giá sau khi hoàn thành chuyến | Khách hàng chỉ được đánh giá tài xế sau khi chuyến đi hoàn thành. |
| BRU13 | Chức năng quản trị phải được phân quyền | Nhân viên chỉ được thực hiện các chức năng phù hợp với quyền được cấp. |
| BRU14 | Các thao tác quan trọng phải được lưu vết | Hệ thống ghi nhận các thao tác quan trọng để phục vụ kiểm tra khi xảy ra sự cố. |

### 2. Ngoại lệ (Exceptions)

| Mã | Ngoại lệ | Cách xử lý |
|---|---|---|
| EX01 | Không xác định được vị trí khách hàng | Yêu cầu khách hàng nhập hoặc chọn điểm đón thủ công. |
| EX02 | Không tìm được tài xế phù hợp | Thông báo cho khách hàng rằng hiện tại không tìm được tài xế. |
| EX03 | Tài xế từ chối chuyến | Hệ thống tự động tìm và gửi yêu cầu đến tài xế khác. |
| EX04 | Tài xế không phản hồi | Sau thời gian phản hồi quy định, hệ thống tiếp tục tìm tài xế khác. |
| EX05 | Tài xế mất kết nối | Ghi nhận tình trạng kết nối và xử lý theo chính sách vận hành. |
| EX06 | Khách hàng mất kết nối | Duy trì trạng thái chuyến và đồng bộ lại thông tin khi khách hàng kết nối lại. |
| EX07 | Thanh toán điện tử thất bại | Thông báo cho khách hàng và cho phép thực hiện lại thanh toán theo chính sách doanh nghiệp. |
| EX08 | Dịch vụ thanh toán gặp lỗi | Không để lỗi thanh toán làm ngừng toàn bộ hệ thống đặt xe. |
| EX09 | Dịch vụ thông báo gặp lỗi | Chuyến đi vẫn tiếp tục hoạt động và hệ thống xử lý việc gửi lại thông báo. |
| EX10 | Dữ liệu nhập không hợp lệ | Thông báo lỗi và yêu cầu người dùng kiểm tra, nhập lại thông tin. |



  # B9: mô hình hoá dữ liệu(data modeling)
 xác định các thực thể
 ví dụ: khách hàng có thuộc tính: id,fullname,email,sdt,..
## Mô hình hóa dữ liệu (Data Modeling)

- Khách hàng (customer_id, full_name, email, phone_number, password, address, status)

- Tài xế (driver_id, full_name, email, phone_number, password, license_number, status, current_location, rating)

- Phương tiện (vehicle_id, driver_id, vehicle_type, license_plate, brand, model, color, status)

- Yêu cầu đặt xe (booking_id, customer_id, pickup_location, destination, vehicle_type, request_time, status)

- Chuyến đi (trip_id, customer_id, driver_id, pickup_location, destination, distance, estimated_time, fare, status, start_time, end_time)

- Thanh toán (payment_id, trip_id, payment_method, amount, payment_status, transaction_code, payment_time)

- Đánh giá (rating_id, trip_id, customer_id, driver_id, score, comment, created_at)

- Thông báo (notification_id, user_id, title, content, notification_type, status, created_at)

- Nhân viên vận hành (operator_id, full_name, email, phone_number, password, role, status)

- Nhật ký hệ thống (log_id, user_id, action, description, created_at)
 
# B10: xác định none functional requirement(yêu cầu phi chức năng)
## Non-Functional Requirement (NFR)

- NFR01: Hệ thống phải hoạt động ổn định khi số lượng người dùng tăng cao.
- NFR02: Hệ thống phải xử lý yêu cầu đặt xe và tìm tài xế trong thời gian hợp lý.
- NFR03: Trạng thái chuyến đi và vị trí tài xế phải được cập nhật gần thời gian thực.
- NFR04: Các thành phần của hệ thống phải có khả năng mở rộng độc lập.
- NFR05: Hệ thống phải dễ dàng bổ sung loại dịch vụ, phương thức thanh toán và kênh thông báo mới.
- NFR06: Lỗi thanh toán hoặc thông báo không được làm toàn bộ hệ thống đặt xe ngừng hoạt động.
- NFR07: Người dùng phải được xác thực trước khi sử dụng các chức năng yêu cầu tài khoản.
- NFR08: Các chức năng quản trị phải được phân quyền.
- NFR09: Dữ liệu cá nhân, vị trí, phương tiện và giao dịch phải được bảo vệ.
- NFR10: Hệ thống không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán.
- NFR11: Các thao tác quan trọng phải được lưu vết.
- NFR12: Các chức năng mới phải có thể triển khai từng phần và hạn chế ảnh hưởng đến hệ thống đang hoạt động.
# B11: VẼ USECASE(UC)
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/e2974959-d634-445e-a63d-89d9d1a4a8ad" />


# B12: Tạo usecase specification( ĐẶC TẢ USECASE)
# ĐẶC TẢ USE CASE (USE CASE SPECIFICATION)

## UC01: Đăng nhập

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC01 |
| Tên Use Case | Đăng nhập |
| Actor | Khách hàng, Tài xế, Nhân viên vận hành/Admin |
| Mô tả | Cho phép người dùng đăng nhập vào hệ thống bằng tài khoản đã đăng ký. |
| Tiền điều kiện | Người dùng đã có tài khoản hợp lệ. |
| Hậu điều kiện | Người dùng đăng nhập thành công và được truy cập vào hệ thống. |
| Trigger | Người dùng chọn chức năng Đăng nhập. |

### Luồng chính
1. Người dùng chọn chức năng Đăng nhập.
2. Hệ thống hiển thị form đăng nhập.
3. Người dùng nhập email/số điện thoại và mật khẩu.
4. Hệ thống kiểm tra thông tin đăng nhập.
5. Hệ thống xác thực tài khoản.
6. Hệ thống cho phép người dùng truy cập.

### Luồng thay thế/Ngoại lệ
- A1: Người dùng nhập thiếu thông tin → Hệ thống yêu cầu nhập đầy đủ.
- A2: Thông tin đăng nhập không chính xác → Hệ thống thông báo đăng nhập thất bại.
- A3: Tài khoản không hoạt động → Hệ thống từ chối đăng nhập.

---

## UC02: Đặt xe

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC02 |
| Tên Use Case | Đặt xe |
| Actor | Khách hàng |
| Mô tả | Cho phép khách hàng nhập điểm đón, điểm đến, lựa chọn loại xe và tạo yêu cầu đặt xe. |
| Tiền điều kiện | Khách hàng đã đăng nhập. |
| Hậu điều kiện | Yêu cầu đặt xe được tạo và hệ thống bắt đầu tìm tài xế. |
| Trigger | Khách hàng chọn chức năng Đặt xe. |

### Luồng chính
1. Khách hàng chọn Đặt xe.
2. Hệ thống xác định vị trí khách hàng.
3. Khách hàng nhập hoặc chọn điểm đón.
4. Khách hàng nhập điểm đến.
5. Khách hàng lựa chọn loại xe.
6. Hệ thống tính khoảng cách từ điểm đón đến điểm đến.
7. Hệ thống hiển thị thông tin chuyến đi.
8. Khách hàng xác nhận đặt xe.
9. Hệ thống tạo yêu cầu đặt xe.
10. Hệ thống bắt đầu tìm tài xế.

### Luồng thay thế/Ngoại lệ
- A1: Không xác định được vị trí → Khách hàng nhập điểm đón thủ công.
- A2: Điểm đón hoặc điểm đến không hợp lệ → Hệ thống yêu cầu nhập lại.
- A3: Chưa chọn loại xe → Hệ thống yêu cầu khách hàng chọn loại xe.

---

## UC03: Tìm và phân công tài xế

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC03 |
| Tên Use Case | Tìm và phân công tài xế |
| Actor | Tài xế |
| Mô tả | Hệ thống tìm tài xế phù hợp và gửi yêu cầu chuyến đến tài xế. |
| Tiền điều kiện | Có yêu cầu đặt xe hợp lệ. |
| Hậu điều kiện | Tài xế được phân công hoặc khách hàng được thông báo không tìm được tài xế. |
| Trigger | Khách hàng xác nhận yêu cầu đặt xe. |

### Luồng chính
1. Hệ thống nhận yêu cầu đặt xe.
2. Hệ thống tìm tài xế đang sẵn sàng.
3. Hệ thống lọc tài xế theo loại xe.
4. Hệ thống xác định vị trí tài xế.
5. Hệ thống tính khoảng cách từ tài xế đến điểm đón.
6. Hệ thống ưu tiên tài xế phù hợp và gần khách hàng.
7. Hệ thống gửi yêu cầu chuyến đến tài xế.
8. Tài xế chấp nhận chuyến.
9. Hệ thống gán tài xế cho chuyến.
10. Hệ thống thông báo cho khách hàng.

### Luồng thay thế/Ngoại lệ
- A1: Tài xế từ chối → Hệ thống tìm tài xế khác.
- A2: Tài xế không phản hồi → Hệ thống chuyển sang tài xế khác.
- A3: Không tìm được tài xế phù hợp → Hệ thống thông báo cho khách hàng.

---

## UC04: Nhận/Từ chối chuyến

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC04 |
| Tên Use Case | Nhận/Từ chối chuyến |
| Actor | Tài xế |
| Mô tả | Cho phép tài xế chấp nhận hoặc từ chối yêu cầu chuyến. |
| Tiền điều kiện | Tài xế đã đăng nhập và đang ở trạng thái sẵn sàng. |
| Hậu điều kiện | Tài xế được gán vào chuyến hoặc hệ thống tìm tài xế khác. |
| Trigger | Tài xế nhận được yêu cầu chuyến mới. |

### Luồng chính
1. Tài xế nhận yêu cầu chuyến.
2. Hệ thống hiển thị thông tin chuyến.
3. Tài xế xem thông tin chuyến.
4. Tài xế chọn Chấp nhận.
5. Hệ thống xác nhận.
6. Hệ thống gán tài xế cho chuyến.
7. Hệ thống thông báo cho khách hàng.

### Luồng thay thế/Ngoại lệ
- A1: Tài xế chọn Từ chối → Hệ thống tìm tài xế khác.
- A2: Tài xế không phản hồi trong thời gian quy định → Hệ thống tìm tài xế khác.
- A3: Chuyến đã được tài xế khác nhận → Hệ thống thông báo chuyến không còn khả dụng.

---

## UC05: Theo dõi và cập nhật trạng thái chuyến đi

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC05 |
| Tên Use Case | Theo dõi và cập nhật trạng thái chuyến đi |
| Actor | Khách hàng, Tài xế |
| Mô tả | Cho phép tài xế cập nhật trạng thái và khách hàng theo dõi quá trình thực hiện chuyến đi. |
| Tiền điều kiện | Chuyến đã được gán cho tài xế. |
| Hậu điều kiện | Trạng thái chuyến được cập nhật đến khi hoàn thành. |
| Trigger | Tài xế bắt đầu thực hiện chuyến. |

### Luồng chính
1. Tài xế di chuyển đến điểm đón.
2. Tài xế cập nhật trạng thái Đã đến điểm đón.
3. Hệ thống thông báo cho khách hàng.
4. Tài xế đón khách.
5. Tài xế cập nhật trạng thái Đã đón khách.
6. Tài xế cập nhật trạng thái Đang di chuyển.
7. Khách hàng theo dõi trạng thái chuyến.
8. Tài xế đến điểm đến.
9. Tài xế cập nhật trạng thái Hoàn thành chuyến.
10. Hệ thống ghi nhận chuyến đã hoàn thành.

### Luồng thay thế/Ngoại lệ
- A1: Tài xế mất kết nối → Hệ thống duy trì trạng thái gần nhất và đồng bộ lại khi có kết nối.
- A2: Khách hàng mất kết nối → Hệ thống tiếp tục lưu trạng thái chuyến và hiển thị lại khi kết nối.

---

## UC06: Thanh toán

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC06 |
| Tên Use Case | Thanh toán |
| Actor | Khách hàng, Nhà cung cấp thanh toán |
| Mô tả | Cho phép khách hàng thanh toán cước chuyến đi bằng tiền mặt hoặc thanh toán điện tử. |
| Tiền điều kiện | Chuyến đi đã hoàn thành. |
| Hậu điều kiện | Kết quả thanh toán được ghi nhận. |
| Trigger | Chuyến đi được hoàn thành. |

### Luồng chính
1. Hệ thống tính cước chuyến đi.
2. Hệ thống hiển thị số tiền phải trả.
3. Khách hàng lựa chọn phương thức thanh toán.
4. Khách hàng chọn thanh toán điện tử.
5. Hệ thống gửi yêu cầu đến nhà cung cấp thanh toán.
6. Nhà cung cấp xử lý giao dịch.
7. Hệ thống nhận kết quả giao dịch.
8. Hệ thống cập nhật trạng thái thanh toán.
9. Hệ thống thông báo kết quả cho khách hàng.

### Luồng thay thế/Ngoại lệ
- A1: Khách hàng chọn tiền mặt → Hệ thống ghi nhận thanh toán bằng tiền mặt.
- A2: Thanh toán điện tử thất bại → Hệ thống thông báo cho khách hàng.
- A3: Thanh toán thất bại → Cho phép khách hàng thực hiện lại theo chính sách.
- A4: Nhà cung cấp thanh toán gặp lỗi → Không làm gián đoạn các chức năng khác của hệ thống.

---

## UC07: Đánh giá tài xế

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC07 |
| Tên Use Case | Đánh giá tài xế |
| Actor | Khách hàng |
| Mô tả | Cho phép khách hàng đánh giá tài xế sau chuyến đi. |
| Tiền điều kiện | Chuyến đi đã hoàn thành. |
| Hậu điều kiện | Đánh giá được lưu vào hệ thống. |
| Trigger | Khách hàng chọn chức năng Đánh giá tài xế. |

### Luồng chính
1. Khách hàng mở chuyến đi đã hoàn thành.
2. Khách hàng chọn Đánh giá tài xế.
3. Hệ thống hiển thị form đánh giá.
4. Khách hàng chọn số điểm.
5. Khách hàng nhập nhận xét nếu có.
6. Khách hàng gửi đánh giá.
7. Hệ thống lưu đánh giá.
8. Hệ thống thông báo đánh giá thành công.

### Luồng thay thế/Ngoại lệ
- A1: Chuyến chưa hoàn thành → Hệ thống không cho phép đánh giá.
- A2: Dữ liệu đánh giá không hợp lệ → Hệ thống yêu cầu nhập lại.

---

## UC08: Quản lý vận hành

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC08 |
| Tên Use Case | Quản lý vận hành |
| Actor | Nhân viên vận hành/Admin |
| Mô tả | Cho phép nhân viên quản lý và giám sát hoạt động của CAB System. |
| Tiền điều kiện | Nhân viên đã đăng nhập và có quyền phù hợp. |
| Hậu điều kiện | Dữ liệu được cập nhật hoặc thông tin được hiển thị theo yêu cầu. |
| Trigger | Nhân viên truy cập chức năng quản lý vận hành. |

### Luồng chính
1. Nhân viên truy cập giao diện quản trị.
2. Hệ thống kiểm tra quyền truy cập.
3. Nhân viên lựa chọn chức năng cần quản lý.
4. Quản lý khách hàng.
5. Quản lý tài xế.
6. Quản lý phương tiện.
7. Quản lý và theo dõi chuyến đi.
8. Tra cứu giao dịch.
9. Xem báo cáo và thống kê.
10. Hệ thống lưu vết các thao tác quan trọng.

### Luồng thay thế/Ngoại lệ
- A1: Nhân viên không có quyền → Hệ thống từ chối thao tác.
- A2: Không tìm thấy dữ liệu → Hệ thống thông báo không có dữ liệu.
- A3: Chuyến gặp sự cố → Nhân viên thực hiện chức năng hỗ trợ xử lý chuyến.

# B13: tiêu chí chấp nhận(AC) (acceptance criteria)
xác nhận chức năng đã đáp ứng yêu cầu khách hàng
ý nghĩa: nhờ nó mà dự án mới được nghiệm thu, cho biết khi nào chức năng hoàn thành và sẵn sàng nghiệm thu)

# TIÊU CHÍ CHẤP NHẬN (ACCEPTANCE CRITERIA)

## UC01: Đăng nhập

- AC01: Người dùng nhập đúng thông tin tài khoản thì đăng nhập thành công.
- AC02: Người dùng nhập sai email/số điện thoại hoặc mật khẩu thì hệ thống hiển thị thông báo lỗi.
- AC03: Người dùng nhập thiếu thông tin bắt buộc thì hệ thống không cho phép đăng nhập.
- AC04: Người dùng đăng nhập thành công được truy cập đúng chức năng theo vai trò của mình.

---

## UC02: Đặt xe

- AC05: Khách hàng có thể xác định hoặc nhập điểm đón.
- AC06: Khách hàng có thể nhập điểm đến.
- AC07: Khách hàng có thể lựa chọn loại xe.
- AC08: Hệ thống xác định được khoảng cách từ điểm đón đến điểm đến.
- AC09: Khách hàng chỉ có thể gửi yêu cầu khi thông tin đặt xe hợp lệ.
- AC10: Sau khi khách hàng xác nhận, hệ thống tạo yêu cầu đặt xe thành công.
- AC11: Sau khi tạo yêu cầu, hệ thống bắt đầu quá trình tìm tài xế.

---

## UC03: Tìm và phân công tài xế

- AC12: Hệ thống chỉ tìm các tài xế đang ở trạng thái sẵn sàng.
- AC13: Hệ thống lọc tài xế phù hợp với loại xe khách hàng lựa chọn.
- AC14: Hệ thống xác định và sử dụng vị trí tài xế để tìm tài xế gần khách hàng.
- AC15: Hệ thống gửi yêu cầu chuyến đến tài xế phù hợp.
- AC16: Khi tài xế chấp nhận, hệ thống gán tài xế vào chuyến.
- AC17: Khi tài xế từ chối hoặc không phản hồi, hệ thống tiếp tục tìm tài xế khác.
- AC18: Khi không tìm được tài xế phù hợp, hệ thống thông báo rõ cho khách hàng.

---

## UC04: Nhận/Từ chối chuyến

- AC19: Tài xế sẵn sàng có thể nhận được yêu cầu chuyến mới.
- AC20: Tài xế có thể xem thông tin của chuyến được đề xuất.
- AC21: Tài xế có thể chấp nhận chuyến.
- AC22: Tài xế có thể từ chối chuyến.
- AC23: Khi tài xế chấp nhận, chuyến được gán cho tài xế đó.
- AC24: Khi tài xế từ chối hoặc không phản hồi trong thời gian quy định, hệ thống tìm tài xế khác.

---

## UC05: Theo dõi và cập nhật trạng thái chuyến đi

- AC25: Tài xế có thể cập nhật trạng thái "Đã đến điểm đón".
- AC26: Tài xế có thể cập nhật trạng thái "Đã đón khách".
- AC27: Tài xế có thể cập nhật trạng thái "Đang di chuyển".
- AC28: Tài xế có thể cập nhật trạng thái "Hoàn thành chuyến".
- AC29: Khách hàng có thể xem trạng thái hiện tại của chuyến.
- AC30: Khách hàng nhận được thông báo khi có thay đổi trạng thái quan trọng của chuyến.

---

## UC06: Thanh toán

- AC31: Hệ thống tính được số tiền phải trả sau khi chuyến đi hoàn thành.
- AC32: Khách hàng có thể lựa chọn thanh toán bằng tiền mặt.
- AC33: Khách hàng có thể lựa chọn thanh toán điện tử.
- AC34: Thanh toán điện tử được xử lý thông qua nhà cung cấp thanh toán bên ngoài.
- AC35: Hệ thống ghi nhận được kết quả thanh toán.
- AC36: Khi thanh toán thành công, hệ thống cập nhật trạng thái thanh toán thành công.
- AC37: Khi thanh toán thất bại, hệ thống thông báo cho khách hàng.
- AC38: Khách hàng có thể thực hiện lại thanh toán thất bại theo chính sách của doanh nghiệp.
- AC39: Hệ thống không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán.

---

## UC07: Đánh giá tài xế

- AC40: Chỉ khách hàng có chuyến đã hoàn thành mới được đánh giá tài xế.
- AC41: Khách hàng có thể chọn mức điểm đánh giá.
- AC42: Khách hàng có thể nhập nhận xét về tài xế.
- AC43: Hệ thống lưu đánh giá thành công.
- AC44: Hệ thống không cho phép đánh giá đối với chuyến chưa hoàn thành.

---

## UC08: Quản lý vận hành

- AC45: Nhân viên vận hành/Admin có thể xem và quản lý khách hàng.
- AC46: Nhân viên vận hành/Admin có thể xem và quản lý tài xế.
- AC47: Nhân viên vận hành/Admin có thể quản lý thông tin phương tiện.
- AC48: Nhân viên vận hành/Admin có thể theo dõi các chuyến đang diễn ra.
- AC49: Nhân viên vận hành/Admin có thể tra cứu lịch sử giao dịch.
- AC50: Nhân viên vận hành/Admin có thể hỗ trợ xử lý chuyến gặp sự cố.
- AC51: Hệ thống chỉ cho phép nhân viên thực hiện chức năng phù hợp với quyền được cấp.
- AC52: Nhân viên có quyền phù hợp có thể xem báo cáo số chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế.
- AC53: Hệ thống lưu vết các thao tác quản trị quan trọng.

- # B14: truy xuất nguồn gốc yêu cầu( traceability requirements)
- rtm( ma trận truy xuất nguồn gốc yêu cầu):

  ## Truy xuất nguồn gốc yêu cầu (Requirement Traceability)

Truy xuất nguồn gốc yêu cầu nhằm đảm bảo mỗi yêu cầu của hệ thống đều xuất phát từ một mục tiêu nghiệp vụ và có chức năng cũng như tiêu chí chấp nhận tương ứng.

**Luồng truy xuất:**

Business Goal (BG) → Business Requirement (BR) → Functional Requirement (FR) → Use Case (UC) → Acceptance Criteria (AC)

### Ma trận truy xuất yêu cầu

| Business Goal | Business Requirement | Functional Requirement | Use Case | Acceptance Criteria |
|---|---|---|---|---|
| BG03: Nâng cao trải nghiệm khách hàng | BR01: Hỗ trợ quy trình đặt xe trực tuyến | FR06-FR11: Xác định vị trí, nhập điểm đón/đến, chọn loại xe, tính khoảng cách, gửi yêu cầu | UC02: Đặt xe | AC05-AC11 |
| BG01, BG02: Tăng hiệu quả phân công và giảm thời gian tìm tài xế | BR02: Tự động hóa tìm và phân công tài xế | FR12-FR17: Tìm tài xế sẵn có, lọc loại xe, xác định vị trí, tính khoảng cách, ưu tiên và gửi yêu cầu | UC03: Tìm và phân công tài xế | AC12-AC18 |
| BG01, BG02 | BR03: Đảm bảo khả năng tìm tài xế liên tục | FR18-FR22: Nhận/từ chối, kiểm tra phản hồi, tìm tài xế khác | UC04: Nhận/Từ chối chuyến | AC19-AC24 |
| BG03: Nâng cao trải nghiệm khách hàng | BR04: Hỗ trợ theo dõi chuyến đi | FR23-FR29: Hiển thị tài xế, ETA và cập nhật trạng thái chuyến | UC05: Theo dõi và cập nhật trạng thái chuyến | AC25-AC30 |
| BG02, BG03 | BR05: Quản lý tài xế và phương tiện | FR30-FR33: Cập nhật, lưu vị trí tài xế và dự kiến thời gian đến | UC03, UC05 | AC14, AC29 |
| BG04: Quản lý thanh toán tập trung | BR06: Quản lý tính cước và thanh toán | FR34-FR40: Tính cước, thanh toán và xử lý kết quả | UC06: Thanh toán | AC31-AC39 |
| BG03 | BR07: Quản lý thông báo | FR41-FR46: Gửi thông báo cho khách hàng và tài xế | UC03, UC05, UC06 | AC18, AC30, AC37 |
| BG03 | BR01: Hỗ trợ quy trình đặt xe | FR47-FR49: Lịch sử chuyến và đánh giá tài xế | UC07: Đánh giá tài xế | AC40-AC44 |
| BG05: Nâng cao hiệu quả vận hành | BR08: Hỗ trợ quản lý và vận hành | FR50-FR57: Quản lý khách hàng, tài xế, phương tiện, chuyến và giao dịch | UC08: Quản lý vận hành | AC45-AC50 |
| BG05 | BR10: Đảm bảo bảo mật và phân quyền | FR58-FR61: Xác thực, phân quyền, kiểm soát truy cập và lưu vết | UC01, UC08 | AC01-AC04, AC51, AC53 |
| BG06: Hỗ trợ quản lý hoạt động kinh doanh | BR09: Hỗ trợ báo cáo kinh doanh | FR62-FR66: Báo cáo chuyến, doanh thu, tỷ lệ hoàn thành/hủy và hiệu quả tài xế | UC08: Quản lý vận hành | AC52 |

