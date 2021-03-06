<h1 align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
  Catppuccin for Joplin
</h1>

<h6 align="center">
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-installation">馃敡 Installation</a>
  路
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-floating-markdown-toc">馃巿 Floating TOC</a>
  路
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-additional-syntax-highlighting">馃帹 Additional highlighting</a>
  路
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-hidden-elements">馃シ Hidden elements</a>
  路
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#%EF%B8%8F-spoilers">猬囷笍 Spoilers</a>
  路
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#%EF%B8%8F-mermaid">馃鈥嶁檧锔? Mermaid</a>
</h6>

![image](https://user-images.githubusercontent.com/23323305/170885382-e6674a5e-2fcb-4d01-9333-28ec9346f8c1.png)

## 馃敡 Installation

### 鉁嶏笍 Install fonts

- Regular: [Fira Sans](https://fonts.google.com/specimen/Fira+Sans)
- Monospace: [Fira Code](https://github.com/tonsky/FiraCode)

### 馃柤锔? Install Theme

1. Open Joplin
2. Go to `Tools` > `Options` > `Appearance` > `Theme`
3. Choose `Dark`
4. Click `Apply`
5. In the same page, Click `Show Advanced Settings`
6. Click `Custom stylesheet for rendered Markdown`
7. Copy [Catppuccin userstyle.css code](https://github.com/sadmice/Catppuccin-Theme-For-Joplin/blob/main/userstyle.css)
8. Paste it on your `userstyle.css`
9. Click `Custom stylesheet for Joplin-wide app styles`
10. Copy [Catppuccin userchrome.css code](https://github.com/sadmice/Catppuccin-Theme-For-Joplin/blob/main/userchrome.css)
11. Paste it on your `userchrome.css`
12. Restart Joplin

## 馃挕 Tips

### 馃巿 Floating Markdown TOC

![2022 05 29-21 16 21 screenshot](https://user-images.githubusercontent.com/23323305/170885590-3068d507-e74a-4f37-9d0a-05d75b49535c.png)

To use the table of contents, you need to:

- Enable toc in your settings
  - Go to `tools` > `Options` > `Markdown`
  - `Enable table of contents extension`
  - Click `Apply`
- Include `[[toc]]` in your markdown
- Hover your mouse over the right side of the render viewer

### 馃帹 Additional syntax highlighting

To see all custom syntax highlighting, you first need to enable it in Joplin:

1. Go to `tools` > `Options` > `Markdown`
   - Enable Mermaid diagrams support
   - Enable ==mark== syntax
   - Enable footnotes
   - Enable table of contents extension
   - Enable abbreviation syntax
   - Enable ++insert++ syntax
2. Click `Apply`

Some of them require the Rich Markdown plugin to see them highlighted in the Markdown Editor

1. Go to `tools` > `Options` > `Plugins`
2. Search the plugin `Rich Markdown`
3. Click `Install`
4. Restart Joplin
5. Go to `tools` > `Options` > `Rich Markdown`
6. Enable the `Add additional CSS classes for enhanced customization`
7. Press `OK`

### 馃シ Hidden elements

Some Joplin's UI elements are hidden by default, but you can return them if you need to.

#### "All Notes" button

Change the `all-notes-button-display` variable on line 32 of userchome.css from `none` to `flex`.

```css
--all-notes-button-display: none; /* hidden */
--all-notes-button-display: flex; /* shown */
```

#### Rich Text Editor Switch

Change the `rich-text-editor-switch-button-display` variable on line 33 of userchome.css from `none` to `flex`.

```css
--rich-text-editor-switch-button-display: none; /* hidden */
--rich-text-editor-switch-button-display: flex; /* shown */
```

#### "New Todo" button

Change the `new-todo-button-display` variable on line 34 of userchome.css from `none` to `flex`.

```css
--new-todo-button-display: none; /* hidden */
--new-todo-button-display: flex; /* shown */
```

### 猬囷笍 Spoilers

![image](https://user-images.githubusercontent.com/23323305/168396760-f56100af-0c14-43f2-9386-d333f07e77db.png)

This theme contains styling for the Spoilers plugin.

1. Go to `tools` > `Options` > `Plugins`
2. Search the plugin `Spoilers`
3. Click `Install`
4. Restart Joplin

### 馃鈥嶁檧锔? Mermaid

![image](https://user-images.githubusercontent.com/23323305/170885879-869d9583-3ad7-463e-a208-a56323941354.png)

To see your mermaid charts better, enable a dark theme for them by including `%%{init: { "theme" : "dark", "flowchart" : { "curve" : "basis" } }%%%` in your mermaid markdown.
