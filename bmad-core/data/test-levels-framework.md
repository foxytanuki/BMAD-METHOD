<!-- Powered by BMAD™ Core -->

# テストレベルフレームワーク

異なるシナリオに対して適切なテストレベル（ユニット、結合、E2E）を決定するための総合ガイド。

## テストレベル決定マトリックス

### ユニットテスト

**使用する場合:**

- 純粋関数とビジネスロジックのテスト
- アルゴリズムの正確性
- 入力検証とデータ変換
- 分離されたコンポーネントのエラーハンドリング
- 複雑な計算や状態マシン

**特徴:**

- 高速実行（即座フィードバック）
- 外部依存なし（DB、API、ファイルシステム）
- 高度に保守可能で安定
- 失敗をデバッグしやすい

**Example scenarios:**

```yaml
unit_test:
  component: 'PriceCalculator'
  scenario: 'Calculate discount with multiple rules'
  justification: 'Complex business logic with multiple branches'
  mock_requirements: 'None - pure function'
```

### 結合テスト

**使用する場合:**

- コンポーネント間相互作用の検証
- データベース操作とトランザクション
- APIエンドポイントコントラクト
- サービス間通信
- ミドルウェアとインターセプターの動作

**特徴:**

- 中程度の実行時間
- コンポーネント境界をテスト
- テストデータベースやコンテナを使用する可能性
- システム結合ポイントを検証

**Example scenarios:**

```yaml
integration_test:
  components: ['UserService', 'AuthRepository']
  scenario: 'Create user with role assignment'
  justification: 'Critical data flow between service and persistence'
  test_environment: 'In-memory database'
```

### エンドツーエンドテスト

**使用する場合:**

- 重要なユーザージャーニー
- システム横断ワークフロー
- 視觚的リグレッションテスト
- コンプライアンスと規制要件
- リリース前の最終検証

**特徴:**

- 低速実行
- 完全なワークフローをテスト
- 完全な環境セットアップが必要
- 最も現実的だが最も脆弱

**Example scenarios:**

```yaml
e2e_test:
  journey: 'Complete checkout process'
  scenario: 'User purchases with saved payment method'
  justification: 'Revenue-critical path requiring full validation'
  environment: 'Staging with test payment gateway'
```

## テストレベル選択ルール

### ユニットテストを選ぶ場合:

- ロジックを分離できる
- 副作用が無い
- 高速フィードバックが必要
- サイクロマティック複雑度が高い

### 結合テストを選ぶ場合:

- 永続化層のテスト
- サービスコントラクトの検証
- ミドルウェア/インターセプターのテスト
- コンポーネント境界が重要

### E2Eテストを選ぶ場合:

- ユーザー向け重要パス
- マルチシステム連携
- 規制コンプライアンスシナリオ
- 視覺的リグレッションが重要

## 避けるべきアンチパターン

- ビジネスロジック検証でのE2Eテスト
- フレームワーク動作のユニットテスト
- サードパーティライブラリの結合テスト
- レベル間での重複カバレッジ

## 重複カバレッジガード

**テストを追加する前に確認:**

1. これはすでに低いレベルでテストされているか？
2. 結合テストの代わりにユニットテストでカバーできるか？
3. E2Eテストの代わりに結合テストでカバーできるか？

**カバレッジ重複が受け入れられる場合:**

- 異なる側面をテスト（ユニット:ロジック、結合:相互作用、e2e:ユーザー体験）
- 深層防御が必要な重要パス
- 以前に壊れた機能のリグレッション防止

## テスト命名規約

- ユニット: `test_{component}_{scenario}`
- 結合: `test_{flow}_{interaction}`
- E2E: `test_{journey}_{outcome}`

## Test ID Format

`{EPIC}.{STORY}-{LEVEL}-{SEQ}`

Examples:

- `1.3-UNIT-001`
- `1.3-INT-002`
- `1.3-E2E-001`
