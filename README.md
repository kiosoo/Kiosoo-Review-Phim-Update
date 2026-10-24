# Kiosoo Video Updates

Kho phát hành chính thức cho Kiosoo Video. Mỗi release gồm bộ cài Windows,
manifest runtime có SHA-256 và các component runtime cài theo nhu cầu.

Không cài Python hệ thống và không yêu cầu quyền ghi vào Program Files. Runtime
được Kiosoo Video quản lý trong `%LOCALAPPDATA%\Kiosoo Video\Runtime`.

## Phát hành

- Runtime (`runtime-manifest.json`, `SHA256SUMS.txt`, `*-runtime-*.zip`) được
  đóng gói bằng `scripts/package-*-runtime.ps1` trong repo ứng dụng và upload
  thủ công lên release.
- Workflow chỉ gắn bộ cài trong `payload/` khi đẩy tag `v*`. Nó không xoá release
  và không ghi đè asset runtime.
