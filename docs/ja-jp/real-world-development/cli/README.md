---
slug: ja-jp/real-world-development/cli
title: "GitHub Copilot CLI"
authors:
  - geektrainer
lastUpdated: 2026-06-30
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** は、ターミナルで GitHub Copilot をエージェント型のコーディング アシスタントとして利用できるようにします。コードベースを探索し、コードを生成し、コマンドを実行し、外部ツールに接続できます。すべてコマンド ラインから行えるため、グラフィカル エディターに切り替えずに作業の流れを保てます。

これらの演習では、Copilot CLI のインストールと認証から始め、カスタム命令でプロジェクトのコンテキストを与えたうえで、プラン モードを使って意図的に機能を実装します。続いて Playwright MCP サーバーを接続し、実際のブラウザーでその機能をテストします。その後、再利用可能な agent skill と custom agent で Copilot を拡張します。最後に、コンテキスト管理、モデル選択、共有に使う slash command を確認し、作成した内容を振り返ります。また、[GitHub Copilot CLI と Foundry を使う全 3 モジュールのオプション シリーズ][foundry]では、モデルを準備し、ホスト型エージェントを構築してデプロイし、サイトに統合できます。

## 演習

| 演習 | トピック | 説明 |
|----------|-------|-------------|
| [0. 前提条件][ex0] | セットアップ | リポジトリと codespace を作成する |
| [1. Copilot CLI をインストールする][ex1] | インストール | Copilot CLI をインストールして認証する |
| [2. スター レーティングを追加する][ex2] | 機能 | UI に星評価を追加してユーザーのフィードバックを受け取る |
| [3. エージェント モード: Plan と Autopilot][ex3] | エージェント | Plan と Autopilot を使って計画と実行を進める |
| [4. カスタム命令で Copilot を導く][ex4] | コンテキスト | プロジェクトに必要な指示を追加して Copilot を導く |
| [5. 品質チェック スキルをカスタマイズして使う][ex5] | スキル | 品質管理用のスキルを拡張して使う |
| [6. Playwright MCP で機能を検証する][ex6] | 外部ツール | Playwright MCP を利用して実際のブラウザーで動作を確認する |
| [7. QA エージェントを作成して使う][ex7] | テスト | 品質保証のためのエージェントを作成して使う |
| [8. フィーチャー PR を作成してマージする][ex8] | ワークフロー | 機能の PR を作成してレビューとマージを進める |
| [9. GitHub Copilot CLI のスラッシュ コマンド][ex9] | CLI 機能 | コンテキスト、モデル、共有、コマンドの使い方を確認する |
| [10. まとめと次のステップ][ex10] | まとめ | 重要な概念と次のステップを振り返る |
| [オプション: Foundry を組み込む][foundry] | ホスト型エージェント | モデルを準備し、エージェントを構築してデプロイし、Web サイトに接続する |

## 前提条件

このワークショップに参加する前に、次を準備してください。

- [ ] **Copilot Student、Pro、Pro+、Business、Enterprise** のいずれかの有効なプランがある GitHub アカウント
- [ ] ターミナル / コマンド ライン操作の基本的な知識
- [ ] インストール済みで設定済みの Git

> [!TIP]
> 有料プランがありませんか。認証済みの学生は [GitHub Education][callout-student-plan-education] を通じて GitHub Copilot を無料で利用できます。**Copilot Student** プランには、このワークショップで使用する agent、MCP、code review、Copilot CLI の機能が含まれているため、すべての harness を完了できます。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> Copilot Business または Copilot Enterprise を使用している場合は、管理者が Copilot CLI を有効にしていることを確認してください。

## はじめる

**[演習 0: 前提条件から始める →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
