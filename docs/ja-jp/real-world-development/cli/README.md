---
slug: ja-jp/real-world-development/cli
title: "GitHub Copilot CLI"
description: "Tailspin Toys の変更を 2 つ実装、検証、公開しながら、Copilot CLI のモード、カスタマイズ、MCP ツール、プルリクエストの自動化について学びます。"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** は、ターミナルで GitHub Copilot をエージェント型のコーディング アシスタントとして利用できるようにします。コードベースを探索し、コードを生成し、コマンドを実行し、外部ツールに接続できます。すべてコマンド ラインから行えるため、グラフィカル エディターに切り替えずに作業の流れを保てます。

このワークショップでは、Tailspin Toys で一連の作業を進めます。GitHub Codespaces でプロジェクトを準備して Copilot CLI をインストールし、基本的な使い方を確認します。星評価を追加してブラウザーで結果を確認し、最初のプルリクエスト (PR) を手動でマージします。次に、フィルタリングの issue から始め、Plan モードで方針を決め、Autopilot モードで実装し、Interactive モードでレビューします。リポジトリの指示を更新し、`quality-checks` スキルをカスタマイズして、Playwright MCP でフィルタリングを確認します。さらに QA エージェントを作成し、変更全体をレビューして Agent Merge でフィルタリングの PR をマージします。

PR は 2 つ作成します。1 つ目は星評価、2 つ目は指示とスキルの更新、QA プロファイル、テストを含むフィルタリングの変更です。フィルタリングと品質確認の作業では、同じ会話とブランチを使って各ツールの学習内容を活用します。また、[GitHub Copilot CLI と Foundry を使う全 3 モジュールのオプション シリーズ][foundry]も利用できます。

## 演習

| 演習 | トピック | 説明 |
|----------|-------|-------------|
| [0. 前提条件][ex0] | セットアップ | リポジトリと Codespace を作成する |
| [1. Copilot CLI をインストールする][ex1] | インストール | Copilot CLI をインストールして認証し、基本的な使い方を確認する |
| [2. 星評価を追加する: すぐできる改善][ex2] | 最初の変更 | 既存の評価と評価がない場合の代替表示を行い、最初の PR をマージする |
| [3. エージェント モード: Plan と Autopilot][ex3] | エージェント モード | issue から機能を計画し、Autopilot で構築して Interactive でレビューする |
| [4. カスタム指示で Copilot を導く][ex4] | コンテキスト | 指示を確認、更新し、フィルタリング作業に適用する |
| [5. quality-checks スキルをカスタマイズして使う][ex5] | 繰り返し実行できるチェック | 既存のスキルを確認し、レポート形式を変更して実行する |
| [6. Playwright MCP で機能を検証する][ex6] | ブラウザーでの確認 | CLI で MCP を設定し、フィルタリングの動作を確認する |
| [7. QA エージェントを作成して使う][ex7] | 要件とカバレッジ | 専門プロファイルを作成して選択し、最終検証の証拠を集める |
| [8. 機能 PR を作成してマージする][ex8] | レビューとマージ | 変更全体をレビューし、PR を作成して Agent Merge を使う |
| [9. GitHub Copilot CLI のスラッシュ コマンド][ex9] | CLI 機能 | コンテキスト、モデル、共有、cloud agent への任意の委任を確認する |
| [10. まとめと次のステップ][ex10] | まとめ | ワークフロー、再利用可能なカスタマイズ、その他のリソースを確認する |
| [オプション: Foundry を組み込む][foundry] | ホスト型エージェント | モデルを準備し、カタログに基づいた Backer Concierge を構築してデプロイし、Web サイトに接続する |

## 前提条件

このワークショップに参加する前に、次を準備してください。

- [ ] **Copilot Student、Pro、Pro+、Business、Enterprise** のいずれかの有効なプランがある GitHub アカウント
- [ ] リポジトリと Codespace を作成する権限
- [ ] ターミナルまたはコマンド ライン操作の基本的な知識

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
