# Music_gen

Music_gen là dự án tạo nhạc tự động bằng công nghệ AI/machine learning. Repo này chứa mã nguồn, dữ liệu và tài liệu hướng dẫn để huấn luyện mô hình và tạo ra đoạn nhạc mới dựa trên đầu vào hoặc tùy chỉnh cá nhân.

## Tính năng chính

- Tạo giai điệu nhạc dựa trên mẫu hoặc tự động.
- Huấn luyện mô hình AI từ dataset nhạc (MIDI/wav/abc notation).
- Cấu hình linh hoạt cho nhiều kiểu nhạc.
- Lưu kết quả đầu ra thành file âm thanh.

## Yêu cầu hệ thống

- Python >= 3.8
- Các thư viện: numpy, torch, tensorflow, librosa, mido, ...
- Máy GPU (khuyến nghị) nếu muốn huấn luyện nhanh.

## Cài đặt & sử dụng

### 1. Clone repo
```bash
git clone https://github.com/xuantrung-DA/Music_gen.git
cd Music_gen
```
### 2. Cài đặt thư viện
```bash
pip install -r requirements.txt
```
### 3. Huấn luyện mô hình (tùy chỉnh tham số trong config)
```bash
python train.py --config configs/config.yaml
```
### 4. Tạo nhạc mới
```bash
python generate.py --input melody.mid --output new_song.wav
```

## Cấu trúc thư mục

- `src/` : Mã nguồn chính
- `configs/` : File cấu hình mô hình
- `data/` : Dữ liệu huấn luyện (không kèm dữ liệu lớn)
- `models/` : Các mô hình đã được lưu
- `outputs/` : Kết quả tạo nhạc

## Đóng góp

- Pull request chào đón!
- Mở issue nếu có bug hoặc ý tưởng cải tiến.

## Tác giả

- xuantrung-DA
