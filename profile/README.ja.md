# vespid-ai

AI エージェント / autonomous agents 向けのオープンソース基盤組織です。

vespid-ai は、trustworthy agent execution に必要なシステム層、つまり agent runtime、delegated authorization、sandboxed execution、protected actions、portable context / memory、operator tooling を中心に構築しています。

本番環境でエージェントを動かすとき、本当に重要なのはモデルの出力品質だけではありません。

- 誰がその操作を承認するのか
- どの境界内で実行されるのか
- コンテキストや memory を安全に持ち運び、監査し、復元できるのか

vespid-ai はこれらをブラックボックスな製品体験として隠すのではなく、明示的で再利用可能なオープンソースのレイヤーとして切り出します。

## 主要リポジトリ

| レイヤー | リポジトリ | 役割 |
| --- | --- | --- |
| Runtime substrate | [`vespid`](https://github.com/vespid-ai/vespid) | brokered sessions、sandboxes、protected actions、再利用可能な agent runtime primitives |
| Delegated authorization | [`skillauth`](https://github.com/vespid-ai/skillauth) | パスワードや cookie を直接共有せずに login-gated platforms へ安全にアクセスするための toolkit |
| Profile portability | [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) | Hermes Agent profile を export / sanitize / sync / restore し、memory・config・sessions・secrets を安全に扱うための基盤 |
| Public docs | [`vespid-ai`](https://github.com/vespid-ai/vespid-ai) | 公開ドキュメント、project index、field notes、そして agent infrastructure の全体像 |

## 何を作っているか

### 1. Agent runtime
AI agents / autonomous agents のための controllable execution environment を作ります。実行、状態、権限を一つの不透明な表面に押し込めません。

### 2. Agent authorization
delegated authorization / scoped access を重視し、人間が信頼できるデバイスで承認し、agent には audit 可能・revoke 可能・短命な capability だけを渡す方向を取ります。

### 3. Portable context and memory
operator context、memory、skills、config、sessions を、一台のマシンに閉じた履歴ではなく、移植可能なシステム資産として扱います。

## 関連する検索トピック

次のような領域に関心がある人に向いています。

- AI agent infrastructure
- autonomous agent runtime
- agent authorization
- delegated authorization
- sandboxed execution
- protected actions
- portable memory
- portable context
- operator tooling
- trustworthy agent systems

## リンク

- Website: [vespid.ai](https://vespid.ai)
- Runtime: [`vespid`](https://github.com/vespid-ai/vespid)
- Authorization: [`skillauth`](https://github.com/vespid-ai/skillauth)
- Portability: [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync)
- English: [README.md](https://github.com/vespid-ai/.github/blob/main/profile/README.md)
- 简体中文: [README.zh-CN.md](https://github.com/vespid-ai/.github/blob/main/profile/README.zh-CN.md)
- Español: [README.es.md](https://github.com/vespid-ai/.github/blob/main/profile/README.es.md)

## ステータス

まだ初期段階ですが、runtime・authorization・context portability を分離して扱う agent infrastructure という方向性は明確です。