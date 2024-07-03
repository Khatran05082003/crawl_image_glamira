#crawl_image_glamira
# Hướng dẫn sử dụng

## Script Scraping Web để Lấy URL và Hình Ảnh

Đoạn script này được thiết kế để thu thập các URL từ các sitemap XML, lấy các hình ảnh từ các URL đó và lưu chúng vào một thư mục cục bộ. Nó sử dụng các thư viện `requests`, `xml.etree.ElementTree` và `BeautifulSoup` để thực hiện các yêu cầu web và phân tích HTML.

### Tổng quan về script
#### Session và Chiến lược Thử lại

Script này sử dụng một phiên làm việc và chiến lược thử lại để xử lý các yêu cầu mạng thất bại. Chiến lược này có thể cố gắng lại nhiều lần khi gặp các mã trạng thái nhất định như 429, 500, 502, 503, và 504.

#### Lấy URL từ Sitemaps

Script được thiết kế để lấy các URL từ một chuỗi các sitemap XML. Các URL này được sử dụng để truy cập và thu thập dữ liệu từ các trang web tương ứng.

#### Lấy nguồn ảnh

Đối với mỗi URL, script phân tích HTML và thu thập tất cả các nguồn ảnh có trong các thẻ `<img>` từ trang web. Các nguồn ảnh này sau đó được lấy về và sử dụng cho mục đích lưu trữ cục bộ.

#### Lưu trữ Ảnh

Các hình ảnh được tải xuống từ các URL thu thập được và sau đó lưu trữ vào một thư mục cục bộ được chỉ định trên hệ thống của bạn.

### How to Run
1. **Copy the script into a Python file, e.g., web_scraper.py.**
2. **Run the script using Python:**
python web_scraper.py

#### Script sẽ xuất ra số lượng URL được tìm thấy, số lượng hình ảnh được tìm thấy, và số lượng hình ảnh duy nhất được lưu trữ. Các hình ảnh sẽ được lưu vào thư mục cục bộ được chỉ định.

### Demo
![image](https://github.com/Khatran05082003/crawl_image_glamira/assets/102920168/3dcc904c-09b2-4234-8635-4e569db7ad85)

![image](https://github.com/Khatran05082003/crawl_image_glamira/assets/102920168/490becd1-65b2-4955-8942-cb32a15b4dbb)

