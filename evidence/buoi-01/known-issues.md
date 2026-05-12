# Known Issues · Buổi 1

Ghi lại lỗi chưa xử lý được hoặc đã xử lý xong.

| STT | Lỗi gặp phải | Lệnh gây lỗi | Cách đã thử | Trạng thái |
|---:|---|---|---|---|
| 1 | | | | |
# Known Issues

* Docker Desktop encountered segmentation fault issues after attempting to pull `ultralytics/ultralytics:latest-cpu`
* Errors observed:

  * `input/output error`
  * `Segmentation fault`
* Cause is likely related to WSL2 overlay filesystem and large PyTorch layers inside the Ultralytics image.
* Other required setup steps, Docker images, and smoke tests were completed successfully before the Docker runtime became unstable.
