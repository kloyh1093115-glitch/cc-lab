# STATE.md テンプレート集

各 STATE.md の初期生成時に使用するテンプレート。
`{{...}}` はオンボーディングデータまたは教授の判断で置換する。

---

## 教授 STATE.md（.lab/STATE.md）

```markdown
# 教授 STATE
最終更新: {{CREATED_DATE}}

## 現在のフェーズ
{{CURRENT_PHASE}}
※ フェーズによって判断基準が変わる：
  - 探索：幅広く仮説を出す
  - 仮説検証：1つの仮説を潰しにいく
  - 論文執筆：新しい実験より整合性を優先

## 研究の全体像
{{RESEARCH_OVERVIEW}}

## 仮説レジストリ
### アクティブ
{{HYPOTHESES}}

### 検証済み
（なし）

## 洞察・アイデアの種
{{INSIGHTS}}

## 次のアクション候補
{{NEXT_ACTIONS}}

## 領域横断の矛盾・未解決の問い
（なし）

## メモ
{{NOTES}}
```

---

## theory/STATE.md

```markdown
# 理論 STATE
最終更新: {{CREATED_DATE}}

## 現在の結論
（なし）

## 関連仮説
（.lab/STATE.md の仮説レジストリを参照）

## 未解決の問い
（なし）

## 矛盾・指摘フラグ
（なし）

## メモ
（なし）

## active/ 参照
（なし）

## archive/ 参照
（なし）
```

---

## experiments/STATE.md

```markdown
# 実験 STATE
最終更新: {{CREATED_DATE}}

## 現在の結論
（なし）

## 実行中ジョブ
（なし）

## 最新の実験結果
（なし）

## 関連仮説
（.lab/STATE.md の仮説レジストリを参照）

## 未解決の問い
（なし）

## 矛盾・指摘フラグ
（なし）

## メモ
（なし）

## active/ 参照
（なし）

## archive/ 参照
（なし）
```

---

## literature/STATE.md

```markdown
# 文献 STATE
最終更新: {{CREATED_DATE}}

## 現在の結論
（なし）

## 最終サーベイ
（未実施）

## 関連仮説
（.lab/STATE.md の仮説レジストリを参照）

## 未解決の問い
（なし）

## 矛盾・指摘フラグ
（なし）

## メモ
{{LITERATURE_NOTES}}

## active/ 参照
（なし）

## archive/ 参照
（なし）
```

---

## paper/STATE.md

※ 論文の話が出るまで作成しない。作成時は教授がヒアリングして埋める。

```markdown
# 論文 STATE
最終更新: {{DATE}}

## 共通認識
- **ターゲット**: {{TARGET_VENUE}}
- **Main contribution**: {{MAIN_CONTRIBUTION}}
- **ストーリーの軸**: {{STORY_AXIS}}

## 構成
| セクション | 状態 | メモ |
|-----------|------|------|
| Abstract | 未着手 | |
| Introduction | 未着手 | |
| Related Work | 未着手 | |
| Method | 未着手 | |
| Experiments | 未着手 | |
| Discussion | 未着手 | |
| Conclusion | 未着手 | |

## 未解決の問い
（なし）
```

---

## log.md 初期状態

```markdown
# 研究ログ

<!-- フォーマット：[日時] [領域] ([方式]): [事実] → [参照先] -->
<!-- 直近2ヶ月分を保持。超過分は log-archive/YYYY-MM.md へ -->

[{{CREATED_DATE}}] [全体] (教授): 研究室セットアップ完了 → .lab/
```
