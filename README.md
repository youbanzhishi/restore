


原始指令

curl -H "这里填 token" \
  -H "Accept: application/vnd.github.v3.raw" \
  https://api.github.com/repos/youbanzhishi/openclaw/contents/restore.sh | bash


加密后的使用方法：
curl -fsSL ”https://raw.githubusercontent.com/youbanzhishi/restore/main/openclaw_restore.enc“ | openssl enc -aes-256-cbc -a -d -pbkdf2 -pass pass:这里填密码 | bash
