<!-- Powered by BMAD™ Core -->

# ストーリードラフトチェックリスト

スクラムマスターは、このチェックリストを使用して、各ストーリーが開発エージェントに成功裏に実装されるのに十分なコンテキストが含まれていることを検証します。この際、開発エージェントが物事を理解する合理的な能力を持っていることを前提とします。

[[LLM: INITIALIZATION INSTRUCTIONS - STORY DRAFT VALIDATION

Before proceeding with this checklist, ensure you have access to:

1. The story document being validated (usually in docs/stories/ or provided directly)
2. The parent epic context
3. Any referenced architecture or design documents
4. Previous related stories if this builds on prior work

IMPORTANT: This checklist validates individual stories BEFORE implementation begins.

VALIDATION PRINCIPLES:

1. Clarity - A developer should understand WHAT to build
2. Context - WHY this is being built and how it fits
3. Guidance - Key technical decisions and patterns to follow
4. Testability - How to verify the implementation works
5. Self-Contained - Most info needed is in the story itself

REMEMBER: We assume competent developer agents who can:

- Research documentation and codebases
- Make reasonable technical decisions
- Follow established patterns
- Ask for clarification when truly stuck

We're checking for SUFFICIENT guidance, not exhaustive detail.]]

## 1. 目標とコンテキストの明確性

[[LLM: Without clear goals, developers build the wrong thing. Verify:

1. The story states WHAT functionality to implement
2. The business value or user benefit is clear
3. How this fits into the larger epic/product is explained
4. Dependencies are explicit ("requires Story X to be complete")
5. Success looks like something specific, not vague]]

- [ ] ストーリーの目標/目的が明確に記述済み
- [ ] エピック目標との関係が明らか
- [ ] ストーリーが全体システムフローにどう組み込まれるかが説明済み
- [ ] 前のストーリーへの依存関係が特定済み（該当する場合）
- [ ] ビジネスコンテキストと価値が明確

## 2. 技術実装ガイダンス

[[LLM: Developers need enough technical context to start coding. Check:

1. Key files/components to create or modify are mentioned
2. Technology choices are specified where non-obvious
3. Integration points with existing code are identified
4. Data models or API contracts are defined or referenced
5. Non-standard patterns or exceptions are called out

Note: We don't need every file listed - just the important ones.]]

- [ ] 作成/修正すべき主要ファイルが特定済み（必ずしも網羅的でなくてよい）
- [ ] このストーリーに特に必要な技術が言及済み
- [ ] 重要なAPIやインターフェースが十分に説明済み
- [ ] 必要なデータモデルや構造が参照済み
- [ ] 必要な環境変数がリスト済み（該当する場合）
- [ ] 標準コーディングパターンへの例外が記述済み

## 3. 参照の有効性

[[LLM: References should help, not create a treasure hunt. Ensure:

1. References point to specific sections, not whole documents
2. The relevance of each reference is explained
3. Critical information is summarized in the story
4. References are accessible (not broken links)
5. Previous story context is summarized if needed]]

- [ ] 外部文書への参照が特定の関連セクションを指定
- [ ] 前のストーリーからの重要情報が要約済み（単に参照するだけではなく）
- [ ] 参照がなぜ関連性があるかのコンテキストが提供済み
- [ ] 参照が一貫したフォーマットを使用（例：`docs/filename.md#section`）

## 4. 自己完結性評価

[[LLM: Stories should be mostly self-contained to avoid context switching. Verify:

1. Core requirements are in the story, not just in references
2. Domain terms are explained or obvious from context
3. Assumptions are stated explicitly
4. Edge cases are mentioned (even if deferred)
5. The story could be understood without reading 10 other documents]]

- [ ] 必要なコア情報が含まれている（外部ドキュメントに過度に依存していない）
- [ ] 暗黙の前提が明示的にされている
- [ ] ドメイン固有の用語や概念が説明済み
- [ ] エッジケースやエラーシナリオが対処済み

## 5. テストガイダンス

[[LLM: Testing ensures the implementation actually works. Check:

1. Test approach is specified (unit, integration, e2e)
2. Key test scenarios are listed
3. Success criteria are measurable
4. Special test considerations are noted
5. Acceptance criteria in the story are testable]]

- [ ] 必要なテストアプローチが概説済み
- [ ] 主要テストシナリオが特定済み
- [ ] 成功基準が定義済み
- [ ] 特別なテスト考慮事項が記述済み（該当する場合）

## 検証結果

[[LLM: FINAL STORY VALIDATION REPORT

Generate a concise validation report:

1. Quick Summary
   - Story readiness: READY / NEEDS REVISION / BLOCKED
   - Clarity score (1-10)
   - Major gaps identified

2. Fill in the validation table with:
   - PASS: Requirements clearly met
   - PARTIAL: Some gaps but workable
   - FAIL: Critical information missing

3. Specific Issues (if any)
   - List concrete problems to fix
   - Suggest specific improvements
   - Identify any blocking dependencies

4. Developer Perspective
   - Could YOU implement this story as written?
   - What questions would you have?
   - What might cause delays or rework?

Be pragmatic - perfect documentation doesn't exist, but it must be enough to provide the extreme context a dev agent needs to get the work down and not create a mess.]]

| カテゴリー                             | ステータス | 問題 |
| ------------------------------------ | ------ | ------ |
| 1. 目標とコンテキストの明確性            | _判定中_  |        |
| 2. 技術実装ガイダンス | _判定中_  |        |
| 3. 参照の有効性           | _判定中_  |        |
| 4. 自己完結性評価       | _判定中_  |        |
| 5. テストガイダンス                  | _判定中_  |        |

**最終評価:**

- 準備完了: ストーリーが実装に十分なコンテキストを提供
- 修正必要: ストーリーの更新が必要（問題を参照）
- ブロック済み: 外部情報が必要（必要な情報を指定）
