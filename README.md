# MMT
CHƯƠNG 1
1
. Mạng máy tính là gì và gồm những thành phần nào? Đây là câu hỏi cơ bản nhất.
•	Định nghĩa: Mạng máy tính là một hệ thống bao gồm các máy tính đơn lẻ (nút mạng) được kết nối với nhau thông qua đường truyền vật lý, theo một kiến trúc xác định và có khả năng trao đổi thông tin.
•	Thành phần chính:
o	Thiết bị đầu cuối (End devices): Là nơi bắt nguồn hoặc nhận dữ liệu (PC, laptop, máy chủ). Trong mạng, chúng đóng vai trò là Server (cung cấp thông tin) hoặc Client (yêu cầu thông tin) hoặc tham gia mạng ngang hàng (Peer-to-Peer).
o	Thiết bị mạng trung gian (Intermediary devices): Nối kết các thiết bị đầu cuối với nhau (Router, Switch, Hub, Firewall). Chúng giúp tái tạo tín hiệu, định tuyến đường đi và thông báo lỗi.
o	Đường truyền vật lý (Network Media): Kênh để truyền thông điệp, bao gồm cáp hữu tuyến (cáp quang, cáp xoắn đôi, cáp đồng trục) và vô tuyến (viba, vệ tinh, wifi).
2. Kiến trúc mạng (Network Architecture) Kiến trúc mạng được định hình bởi hai yếu tố chính: Hình trạng mạng (Topology) và Giao thức mạng (Protocol). Đi kèm với đó là các yêu cầu về Chất lượng dịch vụ (QoS) giúp ưu tiên luồng dữ liệu và Bảo mật mạng (Network Security) với 3 mục tiêu: Bảo mật (Confidentiality), Toàn vẹn (Integrity) và Khả dụng (Availability).
•	Hình trạng mạng (Topology): Là cách thức các nút kết nối với nhau. Các sơ đồ mạng (vật lý và logic) thường dùng các mô hình như hình Sao (Star) có thiết bị trung tâm điều phối, hình lưới (Mesh) độ tin cậy cao dùng cho mạng cốt lõi, mạng dạng tuyến (Bus), dạng vòng (Ring).
•	Giao thức mạng (Protocol): Là tập hợp các quy tắc chi phối việc giao tiếp. Để máy tính hiểu nhau, giao thức phải chuẩn hóa:
o	Mã hóa thông điệp (Encoding): Chuyển đổi dữ liệu thành các tín hiệu điện, ánh sáng hoặc vi sóng phù hợp với đường truyền.
o	Định dạng và đóng gói (Formatting & Encapsulation): Cấu trúc gói tin để truyền đi.
o	Kích thước và thời gian: Phân chia gói tin lớn thành gói nhỏ; quy định thời gian chờ phản hồi và phương thức truy cập đường truyền để tránh xung đột.
o	Phân phối: Gửi đơn hướng (Unicast), đa hướng (Multicast) hoặc quảng bá (Broadcast).
3. Phân loại mạng Đi thi, em thường sẽ gặp các câu hỏi phân biệt các loại mạng. Có 2 tiêu chí phân loại chính:
•	Theo quy mô địa lý: Mạng cục bộ (LAN), Mạng đô thị (MAN), Mạng diện rộng (WAN), Mạng toàn cầu (GAN).
•	Theo kỹ thuật truyền: Đây là phần rất hay thi!
o	Mạng chuyển mạch kênh (Circuit switching): Cấp phát tài nguyên đường truyền dành riêng cho 2 nút mạng. Quá trình gồm 3 bước: thiết lập kênh, truyền dữ liệu, và hủy kênh.
o	Mạng chuyển mạch gói (Packet switching): Thông điệp được chia thành các gói tin nhỏ (packet) chứa địa chỉ đích. Chúng cùng chia sẻ đường truyền, được định tuyến độc lập và có thể đến đích không theo thứ tự. Thiết bị trung gian sử dụng cơ chế lưu trữ và chuyển tiếp (store & forward)
•	Quá trình gửi dữ liệu gọi là đóng gói (Encapsulation) - thêm tiêu đề (header) của từng lớp vào dữ liệu. Quá trình nhận gọi là mở gói (De-encapsulation) - bóc tách dần các tiêu đề.
•	Truyền thông có thể là Hướng liên kết (Connection-oriented) (tin cậy, có thiết lập trước) hoặc Không liên kết (Connectionless) (không cần thiết lập trước, truyền theo "best effort").
Có 2 mô hình cốt lõi em cần nhớ:
1.	Mô hình OSI (7 lớp): Là mô hình tham chiếu lý thuyết. Em cần nhớ tên và chức năng chính của 7 lớp theo thứ tự:
o	Lớp 7 - Ứng dụng (Application): Cung cấp giao diện mạng cho các ứng dụng.
o	Lớp 6 - Trình diễn (Presentation): Đảm bảo định dạng dữ liệu (mã hóa, nén) để các hệ thống hiểu nhau.
o	Lớp 5 - Phiên (Session): Thiết lập, quản lý và kết thúc các phiên giao dịch.
o	Lớp 4 - Giao vận (Transport): Đảm bảo truyền tải dữ liệu tin cậy, sắp xếp gói tin và sửa lỗi.
o	Lớp 3 - Mạng (Network): Xử lý địa chỉ logic (IP) và định tuyến (chọn đường đi) cho gói tin.
o	Lớp 2 - Liên kết dữ liệu (Data Link): Truyền frame tin cậy trên đường truyền vật lý, xử lý địa chỉ vật lý (MAC).
o	Lớp 1 - Vật lý (Physical): Truyền các luồng bit (0,1) thô dưới dạng tín hiệu điện/quang.
2.	Mô hình TCP/IP (4 lớp): Là mô hình thực tế đang được sử dụng cho mạng Internet. Gồm 4 lớp: Ứng dụng (Application), Giao vận (Transport), Internet (tương đương lớp Network của OSI) và Truy nhập mạng (Network Access).
1. Các mô hình tương tác của thiết bị đầu cuối (Host Roles) Trong mạng, các thiết bị đầu cuối giao tiếp với nhau theo hai mô hình chính:
•	Mô hình Khách - Chủ (Client - Server): Server (máy chủ) là máy chạy phần mềm cung cấp thông tin (như Email server, Web server, File server). Client (máy khách) là máy gửi yêu cầu để lấy thông tin từ Server.
•	Mô hình Mạng ngang hàng (Peer-to-Peer - P2P): Một thiết bị có thể vừa đóng vai trò là Client, vừa là Server.
o	Ưu điểm: Dễ cài đặt, ít phức tạp và chi phí thấp, phù hợp cho các tác vụ đơn giản như chia sẻ tệp tin hay máy in.
o	Nhược điểm: Quản trị không tập trung, kém bảo mật, khó mở rộng (không scalable) và hiệu năng thấp. Mô hình này chỉ được khuyến nghị cho các mạng rất nhỏ.
2. Bốn đặc tính cốt lõi của một kiến trúc mạng đáng tin cậy (Reliable Networks) Để mạng hoạt động ổn định và đáp ứng mong đợi của người dùng, kiến trúc mạng phải giải quyết 4 đặc điểm sau:
•	Khả năng chịu lỗi (Fault Tolerance): Mạng phải hạn chế được tác động khi có sự cố bằng cách giới hạn số thiết bị bị ảnh hưởng. Các mạng đáng tin cậy triển khai chuyển mạch gói để tạo ra nhiều đường dẫn dự phòng (redundant connections), giúp gói tin tự động tìm đường khác đi đến đích nếu một liên kết bị đứt.
•	Khả năng mở rộng (Scalability): Mạng có thể mở rộng nhanh chóng để hỗ trợ người dùng mới mà không làm suy giảm hiệu suất của người dùng hiện tại.
•	Chất lượng dịch vụ (QoS): Cơ chế dùng để ưu tiên phân luồng dữ liệu, giúp quản lý lưu lượng hiệu quả. Đi thi, nếu câu hỏi đề cập đến việc xem video trực tiếp hay gọi thoại (VoIP) không bị giật lag, em hãy nhớ ngay đến QoS.
•	Bảo mật mạng (Network Security): Bao gồm bảo vệ phần cứng (ngăn truy cập trái phép thiết bị) và bảo mật thông tin truyền đi. Mục tiêu bảo mật thông tin có 3 yếu tố (CIA): Bảo mật (Confidentiality), Toàn vẹn (Integrity) và Khả dụng (Availability).
3. Môi trường truyền dẫn vật lý (Network Media) Thông điệp từ nguồn đến đích sẽ đi qua các môi trường truyền dẫn, chủ yếu là 3 loại:
•	Cáp kim loại (Cáp đồng): Sử dụng các xung điện để truyền thông tin.
•	Sợi cáp quang (Thủy tinh/Plastic): Sử dụng các xung ánh sáng.
•	Vô tuyến (Wireless): Sử dụng sự điều chế tần số của sóng điện từ (sóng hồng ngoại, viba, vệ tinh).
4. Chi tiết về các yêu cầu của Giao thức mạng (Protocol Requirements) Giao thức quy định cách các thiết bị "nói chuyện" với nhau, bao gồm:
•	Mã hóa thông điệp (Message encoding): Chuyển đổi dữ liệu thành bit, sau đó mã hóa thành mẫu điện áp, xung ánh sáng hoặc vi sóng tùy theo đường truyền.
•	Đóng gói và định dạng (Message formatting): Dữ liệu phải được tuân theo cấu trúc và định dạng nhất định phù hợp với kênh truyền.
•	Kích thước thông điệp (Message size): Một thông điệp dài không thể gửi đi trong một lần mà phải chia thành các phần nhỏ hơn để mạng dễ xử lý, khi đến đích chúng sẽ được tái cấu trúc lại.
•	Thời gian thông điệp (Message timing): Rất quan trọng, gồm Kiểm soát luồng (quản lý lượng dữ liệu và tốc độ truyền) và Phương thức truy cập (xác định thời điểm được phép gửi tín hiệu để tránh xung đột).
•	Tùy chọn phân phối (Message delivery options): Gồm 3 loại chính:
o	Unicast: Gửi từ 1 nguồn đến 1 thiết bị đích.
o	Multicast: Gửi từ 1 nguồn đến một nhóm thiết bị đích.
o	Broadcast: Gửi từ 1 nguồn đến tất cả các thiết bị trên mạng.
5. Kiến trúc Internet và Phân loại mạng nâng cao
•	Thành phần của Internet: Internet là "mạng của các mạng", được chia làm Mạng biên (Network edge) gồm các thiết bị đầu cuối như PC, smartphone, máy chủ; và Mạng lõi (Network core) gồm hệ thống đường truyền và các thiết bị kết nối trung gian (như các trạm chuyển tiếp, router của các nhà cung cấp ISP).
•	Intranet và Extranet:
o	Intranet: Là mạng LAN/WAN nội bộ riêng tư của một tổ chức, chỉ thành viên tổ chức mới truy cập được.
o	Extranet: Mạng cho phép các đối tác/cá nhân bên ngoài có thể truy cập an toàn vào một số dữ liệu nhất định trên mạng nội bộ của tổ chức.
•	Mạng chuyển mạch thông báo (Message switching): Ngoài mạng chuyển mạch kênh và chuyển mạch gói thầy/cô đã nhắc lần trước, còn có mạng chuyển mạch thông báo. Dữ liệu (chứa địa chỉ đích) được truyền theo khối độc lập qua các trạm trung gian. Trạm trung gian sẽ lưu trữ tạm thời và chuyển tiếp (store-and-forward). Kiểu mạng này giúp giảm tắc nghẽn nhưng độ trễ cao, nên không phù hợp với ứng dụng thời gian thực.
1. Phân tích ưu nhược điểm của các Hình trạng mạng (Topology) Hôm trước thầy/cô đã nhắc đến khái niệm, hôm nay chúng ta xét sâu hơn:
•	Mạng dạng vòng (Ring): Các máy được thiết kế thành một vòng khép kín, tín hiệu chạy theo một chiều.
o	Ưu điểm: Tiết kiệm cáp, có thể nới rộng ra xa, tốc độ nhanh hơn Bus.
o	Nhược điểm: Tốc độ nhìn chung vẫn chậm, đặc biệt nếu đứt cáp ở một điểm là toàn bộ mạng ngưng hoạt động, rất khó kiểm tra phát hiện lỗi. Thực tế mạng này ít được sử dụng.
•	Mạng dạng lưới (Mesh): Mỗi một thiết bị sẽ được kết nối với tất cả các thiết bị còn lại.
o	Ứng dụng: Dùng cho các hệ thống tối quan trọng, tuyệt đối không được ngừng hoạt động (ví dụ: nhà máy điện nguyên tử, an ninh, quốc phòng). Đây cũng chính là cấu trúc quen thuộc của Internet.
•	Mạng hình sao mở rộng: Là sự kết hợp của nhiều mạng hình sao thông qua các HUB hoặc Switch.
•	Lưu ý thêm, để quản lý thiết kế mạng, người ta thường dùng 2 loại sơ đồ mạng (Topology diagrams): Sơ đồ vật lý và Sơ đồ logic.
2. Đào sâu về Kỹ thuật truyền số liệu: Chuyển mạch Kênh và Thông báo
•	Mạng chuyển mạch kênh (Circuit Switching): Đây là kỹ thuật cấp phát tài nguyên đường truyền vật lý dành riêng cho 2 nút mạng giao tiếp.
o	Quá trình gồm 3 bước: Thiết lập kênh truyền, truyền dữ liệu, và giải phóng kênh.
o	Ưu điểm: Do đường truyền được giữ riêng trong suốt phiên giao dịch nên đảm bảo chất lượng dịch vụ (QoS), rất phù hợp cho ứng dụng thời gian thực như audio và video.
o	Nhược điểm: Nếu thiết bị chuyển mạch bị lỗi khi đang truyền, quá trình sẽ phải bắt đầu lại từ đầu.
•	Mạng chuyển mạch thông báo (Message Switching):
o	Đặc điểm: Hoàn toàn không thiết lập liên kết dành riêng. Mỗi thông báo mang theo địa chỉ nguồn/đích và truyền đi như một khối độc lập. Các thiết bị trung gian sẽ nhận, lưu trữ rồi chuyển tiếp cho đến khi tới đích.
3. Đơn vị dữ liệu giao thức (PDU) và Truyền thông Logic Để quá trình đóng gói (Encapsulation) và mở gói (De-encapsulation) hoạt động, dữ liệu tại mỗi lớp được xử lý thành các Đơn vị dữ liệu giao thức - PDU (Protocol Data Unit).
•	Một PDU luôn gồm 2 phần: Header (tiêu đề) chứa thông tin điều khiển/địa chỉ và Payload chứa dữ liệu cần truyền tải.
•	Các lớp ngang hàng giữa máy gửi và máy nhận sẽ "nói chuyện" bằng giao thức chung thông qua 2 cách:
o	Hướng liên kết (Connection-oriented): Rất tin cậy, trải qua 3 giai đoạn (thiết lập, truyền, hủy) trên một liên kết đã định sẵn.
o	Hướng không liên kết (Connectionless): Không thiết lập liên kết trước, truyền tin theo kiểu "Best effort" (nỗ lực tối đa), ưu điểm là nhanh nhưng độ tin cậy thấp.
4. Tổ chức mạng Internet
•	Internet được cấu trúc từ việc kết nối các mạng nhỏ vào trạm chuyển tiếp của các ISP (Nhà cung cấp dịch vụ Internet) ở cấp độ khu vực (regional) và toàn cầu (global), thông qua các điểm trung chuyển Internet (IXP).
•	Kiến thức mở rộng: Tại Việt Nam, đơn vị quản lý hoạt động cấp phát tài nguyên địa chỉ Internet quốc gia là VNNIC (Trung tâm Internet Việt Nam).

