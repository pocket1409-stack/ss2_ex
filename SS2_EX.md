### Bước 1: Đề xuất 2 mẫu nhắc nhở (Bài báo: Trích xuất thông tin đánh giá sản phẩm)

-   **Phương án 1 (Đơn giản):**
    
    > "Trích xuất sản phẩm, cảm xúc (tích cực/tiêu cực) và lỗi gặp phải sang JSON từ bình luận: `[Bình luận]`"
    
-   **Phương án 2 (Chi tiết):**
    
    > "Chỉ trả về hợp lệ JSON chuỗi (không giải thích) 
    

### Bước 2: So sánh bảng Sự đánh đổi

**tiêu chí**

**Giải pháp 1 (Đơn giản)**

**Giải pháp 2 (Chi tiết)**

**Độ dễ**

Cao

Trung bình

**Mã thông báo**

Nó

máy bay

**lỗi biên**

Trung bình

vui vẻ

### Bước 3: Lựa chọn và thử nghiệm

-   **Lựa chọn & Lý do:** Chọn **giải pháp 2** vì đảm bảo tính ổn định tuyệt đối cho đầu ra JSON (không kèm theo lời dẫn gây ra hệ thống lỗi) và xử lý tốt các ca thiếu dữ liệu.
    
-   **Chạy thử:**
    
    -   **Đầu vào:** _"Giao hàng siêu nhanh. Máy chạy nhẹ nhưng pin thở hơi nhanh, dùng 3 tiếng là hết."_
        
    -   **Kết quả đầu ra:**
        
        JSON
        
        ```
        {"product": null, "sentiment": "NEU", "issues": ["pin tụt nhanh", "thời lượng pin ngắn (3 tiếng)"]}
        ```
