<!-- ffxiv-tc-port 繁體中文說明開始 -->
# cimplot(台服 fork)

ImPlot（Dear ImGui 的繪圖擴充）的 C API 綁定（上游 [goatcorp/gc-cimplot](https://github.com/goatcorp/gc-cimplot)，再往上是 [cimgui/cimplot](https://github.com/cimgui/cimplot)）。Dalamud 本體把它編成 `cimplot.dll`。

## 台服 fork 的目的

- 讓 Dalamud 本體與這裡的子模組 `implot` 都指向本 org，建置不依賴上游 repo 是否還在、有沒有被改寫。

## 與上游的差異

- 子模組 `implot` 的網址改指 [ffxiv-tc-port/gc-implot](https://github.com/ffxiv-tc-port/gc-implot)。原始碼與上游相同。
- 本分支 `tc-submodule-url` 建在上游較早的 `master` 上，上游之後的更新沒有合入。

## 誰在用它

- [Dalamud](https://github.com/ffxiv-tc-port/Dalamud)：子模組 `lib/cimplot`。

---

以下為上游原始 README，內容未經修改：

<!-- ffxiv-tc-port 繁體中文說明結束 -->
# cimplot

This is a c-api wrapper for implot (https://github.com/epezent/implot) which is a plotter for Dear ImGui (https://github.com/ocornut/imgui)

implot is a submodule of this repo. To do generation again in case implot is changed, you should update implot, make sure that cimgui repository is a sibling folder to this repository folder and execute generator/generator.bat(.sh)
