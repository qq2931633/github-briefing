# Obsidian Git 自动同步配置指南

## 📥 安装步骤

### Step 1: 打开 Obsidian
1. 启动 Obsidian
2. 打开 `github-briefing` vault

### Step 2: 关闭安全模式
1. 左下角点击 **⚙️ 设置 (Settings)**
2. 选择 **第三方插件 (Community Plugins)**
3. 关闭 **安全模式 (Safe Mode)**
4. 点击 **打开社区插件 (Turn on)**

### Step 3: 安装 Git 插件
1. 点击 **浏览 (Browse)**
2. 搜索框输入: `Git`
3. 找到 **Obsidian Git** (作者: Vinzent)
4. 点击 **安装 (Install)**
5. 安装完成后点击 **启用 (Enable)**

### Step 4: 配置自动同步
1. 在设置中找到 **Obsidian Git**
2. 配置以下选项：

**自动 Pull:**
- ✅ Enable Auto Pull: **ON**
- Auto Pull Interval: **3600** (每小时)
- Auto Pull on Startup: **ON**

**自动 Push:**
- ✅ Enable Auto Push: **ON**
- Auto Push Interval: **7200** (每2小时)
- Auto Push on Backup: **ON**

**备份设置:**
- Backup Interval: **30** (每30分钟自动commit)

### Step 5: 首次手动同步
1. 按 `Ctrl+P` (Mac: `Cmd+P`)
2. 输入: `Git: Pull`
3. 选择并执行
4. 等待同步完成

---

## 🔄 使用流程

### 每天早上 (09:00)
1. 打开 Obsidian
2. 自动 pull 最新简报
3. 查看 `daily/日期.md`

### 白天使用
- 在 memos/ 下添加自己的笔记
- Obsidian Git 会自动备份

### 晚上
- 大龙虾 23:00 推送新简报
- 你明天打开就能看到

---

## 📝 常用命令

在 Obsidian 中按 `Ctrl+P` 搜索：

| 命令 | 作用 |
|------|------|
| `Git: Pull` | 拉取最新更新 |
| `Git: Push` | 推送本地修改 |
| `Git: Commit` | 手动提交 |
| `Git: Create Backup` | 立即备份 |

---

## ⚠️ 注意事项

1. **首次使用**需要手动执行一次 `Git: Pull`
2. 如果提示冲突，先备份你的修改，然后重新 pull
3. 保持 Obsidian 打开才能自动同步

---

## 🎯 完成检查清单

- [ ] 安装 Obsidian Git 插件
- [ ] 启用自动 Pull (每小时)
- [ ] 启用自动 Push (每2小时)
- [ ] 执行首次 Git: Pull
- [ ] 测试添加一条笔记看是否自动备份

---

*配置完成后，你的简报会自动同步到所有设备！*
