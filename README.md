# Port & Vessel Tracker (bản online)

Mã nguồn app Streamlit theo dõi cảng biển Việt Nam (12 cảng vụ) + sản lượng container (EconDB) + ước/dự báo hồi quy.
Repo chỉ có **code**; dữ liệu app tự kéo từ Google Drive lúc chạy (secret `RCLONE_CONF` trên Streamlit Cloud).

- Main file: `shipping/port-tracker/app.py`
- Secrets (Streamlit → Settings → Secrets):
  - `RCLONE_CONF = "<base64 của rclone.conf>"` (bắt buộc)
  - `APP_PASSWORD = "<mật khẩu xem app>"` (khuyên dùng: dữ liệu EconDB là gói trả phí)

Mã gốc nằm ở repo private Data-System; repo này được sinh tự động bởi `pack_port_tracker_public.py`, đừng sửa tay.
