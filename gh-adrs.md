# Git Client Architecture Design Record

2025-04-06

### Status

In Progress

### Context

バージョン管理システムを TFS から GitHub へ移行することとなり、GUI クライアントを採用するか、どのツールを使用するかを決定する。
Git の使用経験がない人が多数おり、新しい技術/ツールを使用することをストレスに感じる人もいる。
GitHub Copilot の導入は全員実施しており、Git Cli クライアント導入済み。

### Decision

- Git Cli のみで Git/GitHub によるコーディング手順書を作成する。
  作成後、チームメンバー全員が cli で作業を実施することができ、移行のハードルを超えるか見極める(難易度見極め)
- 難易度高でハードルを超えられないと判断した場合、GUI クライアントを導入することし、評価/選定を行う。
- 選定した GUI クライアントのインストール、初期設定、マニュアルを作成する。
- 上記対応後、チーム内に考えを共有、合意を得てチーム内に周知する。

### Consequences

See Michael Nygard's article, linked above.
