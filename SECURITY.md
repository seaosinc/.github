# Security Policy / セキュリティポリシー

| Item | Detail |
|---|---|
| Scope | Public repositories owned by [SEAOS Inc.](https://github.com/seaosinc) |
| Version | 1.0 |
| Effective | 〈要記入：YYYY-MM-DD〉 |
| Location | `seaosinc/.github` / `SECURITY.md` |
| Precedence | A repository's own `SECURITY.md` takes precedence over this document |

*日本語版は英語版の後に続きます。*

---

## 1. Scope

1.1 This policy applies to all public repositories owned by SEAOS Inc.

1.2 Where a repository provides its own `SECURITY.md`, that document takes precedence.

1.3 Private repositories are governed separately and are not in scope.

## 2. Reporting a vulnerability

2.1 **Do not report vulnerabilities through public issues, pull requests or discussions.** Doing so discloses the attack before a fix is available.

2.2 Reports are accepted through the following channels, in order of preference:

| Priority | Channel |
|---|---|
| 1 | GitHub private vulnerability reporting — **Security → Report a vulnerability** on the affected repository |
| 2 | Email — 〈To be completed: address to be published later〉 |

2.3 Reports may be submitted in English or Japanese.

## 3. Information to include

A report should contain:

- The affected repository, file or path, and the commit where known
- The class of vulnerability (authentication bypass, privilege escalation, information disclosure, injection, supply chain, and so on)
- Steps to reproduce, including the minimal configuration, the input used, and the observed result
- The assessed impact: which actor can reach which asset, and to what extent
- A proposed fix or mitigation, where one is known
- The name under which credit should be given, if desired

## 4. Conduct of research

4.1 Testing shall be conducted only against systems controlled by the reporter. SEAOS production systems and third-party environments are out of scope.

4.2 Where a secret (API key, token, personal data) is reached, only the minimum necessary to demonstrate the finding shall be recorded. Such material shall not be retained, transmitted or used.

4.3 Details shall not be published before a fix is released, in accordance with section 6.

## 5. Response process

| Stage | Target |
|---|---|
| Acknowledgement of receipt | 3 business days |
| Initial assessment (scope and provisional severity) | 7 days |
| Status updates | Every 14 days until resolution |
| Remediation | Critical: 7 days · High: 30 days · Medium: 90 days · Low: next scheduled release |

Severity is assessed with reference to [CVSS v3.1](https://www.first.org/cvss/v3.1/specification-document), taking into account how the affected code is deployed in practice.

Where a report is declined as out of scope, not reproducible or already known, the reason will be provided. A reporter who disagrees with that assessment may request reconsideration.

## 6. Coordinated disclosure

6.1 Reporters are asked to withhold public disclosure until the earlier of 90 days from the report, or the release of a fix.

6.2 Where remediation requires more than 90 days, SEAOS will provide the reason and an estimated timeline, and will agree a disclosure date with the reporter.

6.3 Disclosure is made through GitHub Security Advisories. Credit is given where the reporter wishes.

6.4 Where a reporter discloses in advance of a fix, remediation will nonetheless continue in the interest of users.

## 7. Safe harbour

7.1 SEAOS will not pursue legal action in respect of research and reporting conducted in good faith and in accordance with this policy.

7.2 Where a reporter unintentionally exceeds the scope of this policy, the activity will be treated as good faith provided it is ceased promptly and reported.

7.3 This policy does not authorise attacks on the systems of third parties, nor access to the data of third parties.

## 8. Exclusions

| Out of scope | Refer to |
|---|---|
| Upstream libraries, MCP servers and other dependencies | The respective project |
| GitHub, AWS, Slack and other third-party services | The respective provider |
| SEAOS private repositories | SEAOS internal reporting channel |
| User misconfiguration, except where the design induces the error | — |
| Attacks on third parties, social engineering, physical intrusion, denial of service | Not accepted |

---
---

# 日本語

## 1. 適用範囲

1.1 本ポリシーは、SEAOS Inc. が保有するすべての公開リポジトリに適用する。

1.2 リポジトリ固有の `SECURITY.md` が存在する場合は、当該文書を優先する。

1.3 非公開リポジトリは別途定めるポリシーによるものとし、本ポリシーの対象外とする。

## 2. 脆弱性の報告

2.1 **公開 Issue、プルリクエストおよび Discussions により報告してはならない。** 修正の提供前に攻撃手法が公開されるためである。

2.2 報告は、次の窓口により受け付ける。

| 優先 | 窓口 |
|---|---|
| 1 | GitHub の非公開報告 — 対象リポジトリの **Security → Report a vulnerability** |
| 2 | メール — 〈要記入：アドレスは後日公開〉 |

2.3 報告は日本語または英語による。

## 3. 報告に含める情報

- 対象リポジトリ、ファイルまたはパス（判明している場合はコミット）
- 脆弱性の分類（認証の迂回、権限昇格、情報の露出、インジェクション、供給網等）
- 再現手順（最小構成、入力、観測結果）
- 想定される影響（到達可能な主体、対象資産およびその範囲）
- 判明している場合は、修正案または回避策
- クレジットの記載を希望する場合は、その名義

## 4. 調査に関する遵守事項

4.1 検証は、報告者が管理するシステムにおいてのみ行うものとする。SEAOS の本番環境および第三者の環境は対象外とする。

4.2 秘密情報（API キー、トークン、個人情報）に到達した場合は、立証に必要な最小限の範囲でのみ記録するものとし、保存、転送または利用してはならない。

4.3 修正の公開前に詳細を公表してはならない（第 6 章による）。

## 5. 対応プロセス

| 段階 | 目標 |
|---|---|
| 受領連絡 | 3 営業日 |
| 一次評価（対象の判定および暫定深刻度） | 7 日 |
| 進捗連絡 | 解決まで 14 日ごと |
| 修正完了 | Critical：7 日 ／ High：30 日 ／ Medium：90 日 ／ Low：次回定期リリース |

深刻度は [CVSS v3.1](https://www.first.org/cvss/v3.1/specification-document) を参考とし、実際の配置状況を踏まえて判定する。

対象外、再現不能または既知と判断した場合は、その理由を付して回答する。当該判断に異議がある場合は、再評価を申し出ることができる。

## 6. 協調的開示

6.1 報告から 90 日、または修正の公開のいずれか早い時点まで、詳細の公表を控えるものとする。

6.2 修正に 90 日を超える期間を要する場合は、理由および見込みを通知し、公開時期を協議する。

6.3 公開は GitHub Security Advisory により行い、報告者の希望に応じてクレジットを記載する。

6.4 修正の公開に先立ち報告者が公表した場合においても、利用者保護の観点から修正を継続する。

## 7. セーフハーバー

7.1 本ポリシーに従い誠実に行われた調査および報告について、SEAOS は法的措置を講じない。

7.2 調査の過程で意図せず本ポリシーの範囲を超えた場合においても、速やかに中止し報告されたときは、誠実な調査として取り扱う。

7.3 本ポリシーは、第三者のシステムへの攻撃または第三者のデータへのアクセスを許諾するものではない。

## 8. 適用除外

| 対象外 | 窓口 |
|---|---|
| 依存ライブラリ、MCP サーバその他の依存コンポーネント | 各プロジェクト |
| GitHub、AWS、Slack 等の外部サービス | 各提供者 |
| SEAOS の非公開リポジトリ | 社内の報告窓口 |
| 利用者の設定誤り。ただし設計が当該誤りを誘発する場合を除く | — |
| 第三者への攻撃、ソーシャルエンジニアリング、物理的侵入、サービス妨害 | 受け付けない |

---

## 改訂履歴 / Revision history

| 版 / Version | 日付 / Date | 内容 / Change |
|---|---|---|
| 1.0 | 〈要記入〉 | 制定 / Initial issue |
