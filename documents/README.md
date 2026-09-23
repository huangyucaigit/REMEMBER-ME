# 正式文书版本登记

> 这里登记正式 Word/PDF 文书的版本、用途和校验值。  
> 由于当前 GitHub 连接器仅支持直接写入 UTF-8 文本，二进制 DOCX 本体暂未通过连接器上传；仓库内已保存对应的 Markdown 模板和法规结构。后续二进制文件上传后，应以本页 SHA-256 校验是否为同一版本。

## 当前最新版

### 《关于云灵猴AI编程业务的书面核查与信息查阅申请_第二次修订版.docx》

- **版本状态**：当前正式最新版
- **生成日期**：2026-09-23
- **本地文件大小**：约 48 KB
- **SHA-256**：`585499a81e76b2a6245a181700c08bb5a4e65717752a5d5a05f309b18f44a6e3`
- **GitHub 二进制本体**：**待上传**
- **对应可编辑文本模板**：[templates/移动书面核查与信息查阅申请.md](../templates/移动书面核查与信息查阅申请.md)
- **对应法规说明**：[docs/LEGAL_BASIS.md](../docs/LEGAL_BASIS.md)
- **对应完整订购证据清单**：[docs/SUBSCRIPTION_EVIDENCE_CHECKLIST.md](../docs/SUBSCRIPTION_EVIDENCE_CHECKLIST.md)

## 校验方法

Windows PowerShell：

```powershell
Get-FileHash ".\关于云灵猴AI编程业务的书面核查与信息查阅申请_第二次修订版.docx" -Algorithm SHA256
```

输出应为：

```text
585499a81e76b2a6245a181700c08bb5a4e65717752a5d5a05f309b18f44a6e3
```

## 上传规则

正式 DOCX 上传到仓库后，建议路径：

```text
documents/关于云灵猴AI编程业务的书面核查与信息查阅申请_第二次修订版.docx
```

上传后必须：
1. 核对 SHA-256；
2. 更新本页“GitHub 二进制本体”为“已上传”；
3. 在 `CHANGELOG.md` 记录版本；
4. 后续新版本不得覆盖旧版本，应保留版本历史。