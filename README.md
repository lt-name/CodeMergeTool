# CodeMergeTool 🚀

用于软著申请的代码合并与提取工具 📝

------

## 📖 项目概述

**CodeMergeTool** 是一个专为软著申请设计的代码合并与提取工具，能够自动合并指定类型的代码文件，并提取前1500行和最后1500行代码生成 Word 文档，方便软著申请时的代码整理。

------

## 🔍 功能特点

- 🔗 支持合并多种类型的代码文件（例如 `.ts`、`.js`、`.json` 等）
- 📝 自动过滤注释和空行，提高代码整理的简洁性
- 📄 生成两个 Word 文档，分别包含合并代码的前1500行和最后1500行
- ⚙️ 配置简单，用户可以自定义文件类型和路径
- 🌐 适用于多种编程语言的代码整理需求

------

## 🌐 环境要求

- **Python**: 3.10 及以上
- **依赖库**: `python-docx`, `dotenv`

### 🛠️ 安装依赖

在项目目录下运行以下命令来安装必要的依赖库：

```
pip install python-docx python-dotenv
```

------

## 🚀 使用方法

1. 在项目根目录中找到 `config.json` 文件，复制一份并将其重命名为 `config_file.json`。
2. 根据需要修改 `config_file.json` 中的配置信息。
3. 在终端中运行 `code_merge_tool.py` 脚本，工具会自动合并代码并生成 Word 文档。

### 🏃 运行命令

```
python code_merge_tool.py
```

------

## ⚙️ 配置文件说明

自定义项目配置时，请将 `config.json` 文件复制一份并重命名为 `config_file.json`，然后按照自身需求进行修改。

### `config_file.json` 配置项示例

```
{
    "_comment_PROJECT_ROOT": "项目根目录或代码存放目录",
    "PROJECT_ROOT": "./YourProjectPath",

    "_comment_OUTPUT_DIR": "输出生成文件的目录，默认为 ./Code 文件夹",
    "OUTPUT_DIR": "./Code",

    "_comment_ALL_CODE_FILE": "合并后的代码文件名称",
    "ALL_CODE_FILE": "All_code.txt",

    "_comment_OUTPUT_FIRST_DOC": "保存前1500行代码的文件名称",
    "OUTPUT_FIRST_DOC": "first_1500_lines.docx",

    "_comment_OUTPUT_LAST_DOC": "保存最后1500行代码的文件名称",
    "OUTPUT_LAST_DOC": "last_1500_lines.docx",

    "_comment_FILE_TYPES": "要处理的代码文件类型",
    "FILE_TYPES": [".ts", ".ets", ".js", ".json", ".json5"]
}
```

### 🔧 配置项说明

- **PROJECT_ROOT**: 项目根目录或代码存放的主目录，指定待合并的代码文件所在位置。
- **OUTPUT_DIR**: 输出生成文件的目录，默认为 `Code` 文件夹。
- **ALL_CODE_FILE**: 合并后保存所有代码的文件名称。
- **OUTPUT_FIRST_DOC** 和 **OUTPUT_LAST_DOC**: 生成的 Word 文档文件名称，分别用于保存前1500行和最后1500行代码。
- **FILE_TYPES**: 需要处理的代码文件类型，可以根据需求调整。

------

## 📂 文件结构

```
/YourProjectPath
│
├── config.json                     # 默认配置文件模板
├── config_file.json                # 用户自定义配置文件（按需修改）
├── code_merge_tool.py              # 主工具脚本
├── .gitattributes                  # 不必理会
├── Code/                           # 默认输出目录
│   ├── All_code.txt                # 合并后的所有代码文件
│   ├── first_1500_lines.docx       # 前1500行代码
│   └── last_1500_lines.docx        # 后1500行代码
```

- **config.json**: 默认配置文件模板，请至少更换您的项目目录。
- **config_file.json**: 复制自 `config.json` 的用户自定义配置文件，可根据需求自定义修改。
- **code_merge_tool.py**: 主工具脚本，包含代码合并和生成 Word 文档的逻辑。
- **Code/**: 默认输出目录，存放生成的文件。

------

## 📜 许可证

本项目采用 MIT License 开源，您可以自由使用、修改和分发此代码。

------

## 💬 交流与反馈

如有任何疑问或建议，请通过以下方式联系我们：

- **GitHub Issues**: 提交问题和建议
- **Email**: chayunyolong@gmail.com

希望此工具能够帮助您在软著申请过程中更轻松地整理代码！🙌

------

## ⭐️ 支持我们

如果你觉得这个项目对你有帮助，欢迎给我们一个 ⭐️ Star！这将帮助我们获得更多的支持，也能激励我们持续改进这个项目。
点击右上角的 **Star** 按钮⭐️！

------

