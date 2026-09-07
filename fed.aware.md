# FDE Aware — 業界ドメイン別の観測レンズ

## 定義

**Aware = 何に気づき、何に注意を向けるか。**

FDEにおけるAwareは、SkillやToolではない。現場を観察するときに、どこへ注意を向けるかを決める観測レンズである。

```text
Domain → Aware → Observe → Data → Issue → Agent
```

- **Aware** — Attention Target
- **Skill** — Action Capability over Attention
- **Tool** — Means of Execution
- **Agent** — Problem Solver

勘や経験は「何を観測するか」を決める初期仮説になり得る。しかし、勘そのものを証拠や真実として扱わない。

## 6業界ドメイン

FDEの初期標準として、業界ドメインを6つに限定する。

### 1. Manufacturing — 製造業

```yaml
aware:
  - process
  - machine
  - material
  - quality
  - people
  - flow
```

見るもの：工程、設備、材料、品質、人、流れ。

### 2. Construction — 建設業

```yaml
aware:
  - site
  - structure
  - worker
  - material
  - safety
  - progress
```

見るもの：現場、構造物、作業者、資材、安全、進捗。

### 3. Logistics — 物流

```yaml
aware:
  - inventory
  - shipment
  - route
  - vehicle
  - warehouse
  - time
```

見るもの：在庫、出荷、経路、車両、倉庫、時間。

### 4. Retail — 小売

```yaml
aware:
  - customer
  - product
  - inventory
  - sales
  - store
  - demand
```

見るもの：顧客、商品、在庫、売上、店舗、需要。

### 5. Healthcare — 医療・福祉

```yaml
aware:
  - patient
  - symptom
  - treatment
  - staff
  - facility
  - outcome
```

見るもの：患者、症状、治療、職員、施設、結果。

### 6. Information — 情報通信・IT

```yaml
aware:
  - system
  - data
  - user
  - code
  - service
  - incident
```

見るもの：システム、データ、ユーザー、コード、サービス、障害。

## FDEとの関係

AwareはAgentを先に作るための分類ではない。

```text
WORLD
  ↓
FDE
  ↓
DOMAIN
  ↓
AWARE
  ↓
「何を見るか」
  ↓
OBSERVATION
  ↓
DATA
  ↓
ISSUE
  ↓
AGENT
  ↓
TOOL
  ↓
ACTION
```

つまり、**データが先にあり、そこからIssueが見出され、問題を解決するAgentがやってくる。**

## 製造業を原型とする

この6ドメインの中では、製造業をFDEの基本形として扱う。

```text
製造
  ↓
現場を見る
  ↓
工程・設備・材料・品質・人・流れ
  ↓
データを取る
  ↓
問題を見出す
  ↓
世界をモデリングする
  ↓
解法を設計する
  ↓
実装する
  ↓
運用する
  ↓
改善・再構成する
```

製造業で成立した観測モデルを、建設・物流・小売・医療・ITへ展開する。

## Awareは固定された本質ではない

業界ドメインは世界そのものではない。ミッションに応じて選ばれる観測上のスコープである。

また、Awareも永遠に固定された分類ではない。

```text
観察
 ↓
証拠
 ↓
新しい違和感
 ↓
新しいデータ
 ↓
Awareの追加・変更
 ↓
新しいIssue
```

したがって、ドメインやAwareは現場の証拠によって改善・再構成され得る。

## 6フェーズとの接続

```text
1 OBSERVE
  Domain / Aware を選び、現場を見る
       ↓
2 ISSUE
  Dataから問題を見出す
       ↓
3 MODEL + SOLUTION
  対象世界を限定し、解法まで設計する
       ↓
4 IMPLEMENT
  解法を実装する
       ↓
5 OPERATE
  現実で運用し、結果を観測する
       ↓
6 IMPROVE + RECONFIGURE
  Aware・Model・Solution・Workflowを改善する
       ↺
```

## 原則

1. Awareは観測対象であり、能力ではない。
2. DomainはAgentの身分ではなく、観測コンテキストである。
3. 勘は観測対象を選ぶ仮説であり、真実ではない。
4. EvidenceはInterpretationより先に置く。
5. Issueは観測されたDataから見出される。
6. AgentはIssueの後にやってくる。
7. ToolはAgentが使う手段である。
8. Codingは最初ではなく、Solutionの後のImplementationである。
9. Awareは現場の証拠によって追加・変更できる。
10. 6業界は初期スコープであり、世界そのものではない。

## Core statement

> **FDE Awareとは、業界というスコープの中で、現実のどこに注意を向けるかを定義する観測レンズである。**
