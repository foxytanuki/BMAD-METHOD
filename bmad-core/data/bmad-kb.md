<!-- Powered by BMAD™ Core -->

# BMAD™ ナレッジベース

## 概要

BMAD-METHOD™（Breakthrough Method of Agile AI-driven Development）は、AIエージェントとアジャイル開発手法を組み合わせたフレームワークです。v4システムでは、改善された依存管理、バンドル最適化、Webと統合開発環境（IDE）の両方のサポートを備えたモジュラーアーキテクチャを導入しています。

### 主要機能

- **モジュラーエージェントシステム**: 各アジャイル役割用の専門AIエージェント
- **ビルドシステム**: 自動化された依存関係解決と最適化
- **デュアル環境サポート**: WebUIとIDEの両方に最適化
- **再利用可能リソース**: ポータブルテンプレート、タスク、チェックリスト
- **スラッシュコマンド統合**: 迅速なエージェント切り替えと制御

### BMadを使用する場面

- **新規プロジェクト（グリーンフィールド）**: 完全なエンドツーエンド開発
- **既存プロジェクト（ブラウンフィールド）**: 機能追加と拡張
- **チーム協働**: 複数の役割が協力
- **品質保証**: 構造化されたテストと検証
- **文書化**: プロフェッショナルなPRD、アーキテクチャドキュメント、ユーザーストーリー

## BMadの動作原理

### コアメソッド

BMadはあなたを「Vibe CEO」に変身させ、構造化されたワークフローを通じて専門AIエージェントのチームを指揮します。方法は以下の通りです：

1. **あなたが指揮、AIが実行**: あなたがビジョンと決定を提供し、エージェントが実装詳細を処理
2. **専門エージェント**: 各エージェントが1つの役割をマスター（PM、開発者、アーキテクト等）
3. **構造化ワークフロー**: 実証済みパターンがアイデアからデプロイ済みコードまで導く
4. **クリーンな引き継ぎ**: 新しいコンテキストウィンドウがエージェントの集中と効果を保証

### 2段階アプローチ

#### フェーズ1: 計画（Web UI - コスト効率的）

- 大規模コンテキストウィンドウを使用（Geminiの1Mトークン）
- 包括的文書を生成（PRD、アーキテクチャ）
- ブレインストーミングに複数エージェントを活用
- 一度作成し、開発全体を通して使用

#### フェーズ2: 開発（IDE - 実装）

- 文書を管理可能な断片に分割
- 集中的なSM → Dev サイクルを実行
- 一度に1つのストーリー、順次進行
- リアルタイムファイル操作とテスト

### 開発ループ

```text
1. SMエージェント（新しいチャット） → 分割されたドキュメントから次のストーリーを作成
2. あなた → ストーリーをレビューし承認
3. Devエージェント（新しいチャット） → 承認されたストーリーを実装
4. QAエージェント（新しいチャット） → コードをレビューしリファクタリング
5. あなた → 完了を検証
6. エピックが完了するまで繰り返し
```

### なぜこの方法が機能するか

- **コンテキスト最適化**: クリーンなチャット = より良いAIパフォーマンス
- **役割の明確性**: エージェントがコンテキスト切り替えしない = 高品質
- **漸進的進歩**: 小さなストーリー = 管理可能な複雑さ
- **人間の監視**: あなたが各ステップを検証 = 品質管理
- **文書主導**: 仕様がすべてをガイド = 一貫性

## 始め方

### クイックスタートオプション

#### オプション1: Web UI

**最適**: すぐに始めたいChatGPT、Claude、Geminiユーザー

1. `dist/teams/`に移動
2. `team-fullstack.txt`の内容をコピー
3. 新しいGemini GemまたはCustomGPTを作成
4. 指示と共にファイルをアップロード: 「あなたの重要な操作指示が添付されています。指示された通りにキャラクターを破らないでください」
5. `/help`と入力して利用可能なコマンドを確認

#### Option 2: IDE Integration

**Best for**: Cursor, Claude Code, Windsurf, Trae, Cline, Roo Code, Github Copilot users

```bash
# Interactive installation (recommended)
npx bmad-method install
```

**Installation Steps**:

- Choose "Complete installation"
- Select your IDE from supported options:
  - **Cursor**: Native AI integration
  - **Claude Code**: Anthropic's official IDE
  - **Windsurf**: Built-in AI capabilities
  - **Trae**: Built-in AI capabilities
  - **Cline**: VS Code extension with AI features
  - **Roo Code**: Web-based IDE with agent support
  - **GitHub Copilot**: VS Code extension with AI peer programming assistant
  - **Auggie CLI (Augment Code)**: AI-powered development environment

**Note for VS Code Users**: BMAD-METHOD™ assumes when you mention "VS Code" that you're using it with an AI-powered extension like GitHub Copilot, Cline, or Roo. Standard VS Code without AI capabilities cannot run BMad agents. The installer includes built-in support for Cline and Roo.

**Verify Installation**:

- `.bmad-core/` folder created with all agents
- IDE-specific integration files created
- All agent commands/rules/modes available

**Remember**: At its core, BMAD-METHOD™ is about mastering and harnessing prompt engineering. Any IDE with AI agent support can use BMad - the framework provides the structured prompts and workflows that make AI development effective

### Environment Selection Guide

**Use Web UI for**:

- Initial planning and documentation (PRD, architecture)
- Cost-effective document creation (especially with Gemini)
- Brainstorming and analysis phases
- Multi-agent consultation and planning

**Use IDE for**:

- Active development and coding
- File operations and project integration
- Document sharding and story management
- Implementation workflow (SM/Dev cycles)

**Cost-Saving Tip**: Create large documents (PRDs, architecture) in web UI, then copy to `docs/prd.md` and `docs/architecture.md` in your project before switching to IDE for development.

### IDE-Only Workflow Considerations

**Can you do everything in IDE?** Yes, but understand the tradeoffs:

**Pros of IDE-Only**:

- Single environment workflow
- Direct file operations from start
- No copy/paste between environments
- Immediate project integration

**Cons of IDE-Only**:

- Higher token costs for large document creation
- Smaller context windows (varies by IDE/model)
- May hit limits during planning phases
- Less cost-effective for brainstorming

**Using Web Agents in IDE**:

- **NOT RECOMMENDED**: Web agents (PM, Architect) have rich dependencies designed for large contexts
- **Why it matters**: Dev agents are kept lean to maximize coding context
- **The principle**: "Dev agents code, planning agents plan" - mixing breaks this optimization

**About bmad-master and bmad-orchestrator**:

- **bmad-master**: CAN do any task without switching agents, BUT...
- **Still use specialized agents for planning**: PM, Architect, and UX Expert have tuned personas that produce better results
- **Why specialization matters**: Each agent's personality and focus creates higher quality outputs
- **If using bmad-master/orchestrator**: Fine for planning phases, but...

**CRITICAL RULE for Development**:

- **ALWAYS use SM agent for story creation** - Never use bmad-master or bmad-orchestrator
- **ALWAYS use Dev agent for implementation** - Never use bmad-master or bmad-orchestrator
- **Why this matters**: SM and Dev agents are specifically optimized for the development workflow
- **No exceptions**: Even if using bmad-master for everything else, switch to SM → Dev for implementation

**Best Practice for IDE-Only**:

1. Use PM/Architect/UX agents for planning (better than bmad-master)
2. Create documents directly in project
3. Shard immediately after creation
4. **MUST switch to SM agent** for story creation
5. **MUST switch to Dev agent** for implementation
6. Keep planning and coding in separate chat sessions

## Core Configuration (core-config.yaml)

**New in V4**: The `bmad-core/core-config.yaml` file is a critical innovation that enables BMad to work seamlessly with any project structure, providing maximum flexibility and backwards compatibility.

### What is core-config.yaml?

This configuration file acts as a map for BMad agents, telling them exactly where to find your project documents and how they're structured. It enables:

- **Version Flexibility**: Work with V3, V4, or custom document structures
- **Custom Locations**: Define where your documents and shards live
- **Developer Context**: Specify which files the dev agent should always load
- **Debug Support**: Built-in logging for troubleshooting

### Key Configuration Areas

#### PRD Configuration

- **prdVersion**: Tells agents if PRD follows v3 or v4 conventions
- **prdSharded**: Whether epics are embedded (false) or in separate files (true)
- **prdShardedLocation**: Where to find sharded epic files
- **epicFilePattern**: Pattern for epic filenames (e.g., `epic-{n}*.md`)

#### Architecture Configuration

- **architectureVersion**: v3 (monolithic) or v4 (sharded)
- **architectureSharded**: Whether architecture is split into components
- **architectureShardedLocation**: Where sharded architecture files live

#### Developer Files

- **devLoadAlwaysFiles**: List of files the dev agent loads for every task
- **devDebugLog**: Where dev agent logs repeated failures
- **agentCoreDump**: Export location for chat conversations

### Why It Matters

1. **No Forced Migrations**: Keep your existing document structure
2. **Gradual Adoption**: Start with V3 and migrate to V4 at your pace
3. **Custom Workflows**: Configure BMad to match your team's process
4. **Intelligent Agents**: Agents automatically adapt to your configuration

### Common Configurations

**Legacy V3 Project**:

```yaml
prdVersion: v3
prdSharded: false
architectureVersion: v3
architectureSharded: false
```

**V4 Optimized Project**:

```yaml
prdVersion: v4
prdSharded: true
prdShardedLocation: docs/prd
architectureVersion: v4
architectureSharded: true
architectureShardedLocation: docs/architecture
```

## コア哲学

### Vibe CEOとしての行動

あなたは「Vibe CEO」です - 無制限のリソースと単一のビジョンを持つCEOのように考えてください。AIエージェントはあなたの高機能チームであり、あなたの役割は：

- **指揮**: 明確な指示と目標を提供
- **洗練**: 品質達成のためにアウトプットを反復改善
- **監督**: 全エージェント間で戦略的整合性を維持

### コア原則

1. **AI活用の最大化**: AIにより多くを提供させる。アウトプットに挑戦し反復改善。
2. **品質管理**: あなたが品質の最終判断者。全アウトプットをレビュー。
3. **戦略的監督**: 高レベルビジョンを維持し整合性を保証。
4. **反復改善**: ステップを見直すことを期待。これは線形プロセスではない。
5. **明確な指示**: 精密な要求がより良いアウトプットにつながる。
6. **文書化の重要性**: 良い入力（ブリーフ、PRD）が良いアウトプットにつながる。
7. **小さく始め、素早くスケール**: 概念をテストし、その後拡張。
8. **混乱を受け入れる**: 適応し、課題を克服。

### Key Workflow Principles

1. **Agent Specialization**: Each agent has specific expertise and responsibilities
2. **Clean Handoffs**: Always start fresh when switching between agents
3. **Status Tracking**: Maintain story statuses (Draft → Approved → InProgress → Done)
4. **Iterative Development**: Complete one story before starting the next
5. **Documentation First**: Always start with solid PRD and architecture

## Agent System

### コア開発チーム

| エージェント       | 役割               | 主要機能                       | 使用タイミング                            |
| ----------- | ------------------ | --------------------------------------- | -------------------------------------- |
| `analyst`   | ビジネスアナリスト   | 市場調査、要件収集 | プロジェクト計画、競合分析 |
| `pm`        | プロダクトマネージャー    | PRD作成、機能優先順位付け    | 戦略計画、ロードマップ           |
| `architect` | ソリューションアーキテクト | システム設計、技術アーキテクチャ   | 複雑システム、スケーラビリティ計画  |
| `dev`       | 開発者          | コード実装、デバッグ          | 全開発タスク                  |
| `qa`        | QAスペシャリスト      | テスト計画、品質保証        | テスト戦略、バグ検証     |
| `ux-expert` | UXデザイナー        | UI/UX設計、プロトタイプ                | ユーザー体験、インターフェース設計      |
| `po`        | プロダクトオーナー      | バックログ管理、ストーリー検証    | ストーリー精密化、受入基準  |
| `sm`        | スクラムマスター       | スプリント計画、ストーリー作成         | プロジェクト管理、ワークフロー           |

### メタエージェント

| エージェント               | 役割             | 主要機能                     | 使用タイミング                       |
| ------------------- | ---------------- | ------------------------------------- | --------------------------------- |
| `bmad-orchestrator` | チームコーディネーター | マルチエージェントワークフロー、役割切り替え | 複雑なマルチロールタスク          |
| `bmad-master`       | ユニバーサルエキスパート | 切り替えなしの全機能    | シングルセッション包括作業 |

### Agent Interaction Commands

#### IDE-Specific Syntax

**Agent Loading by IDE**:

- **Claude Code**: `/agent-name` (e.g., `/bmad-master`)
- **Cursor**: `@agent-name` (e.g., `@bmad-master`)
- **Windsurf**: `/agent-name` (e.g., `/bmad-master`)
- **Trae**: `@agent-name` (e.g., `@bmad-master`)
- **Roo Code**: Select mode from mode selector (e.g., `bmad-master`)
- **GitHub Copilot**: Open the Chat view (`⌃⌘I` on Mac, `Ctrl+Alt+I` on Windows/Linux) and select **Agent** from the chat mode selector.

**Chat Management Guidelines**:

- **Claude Code, Cursor, Windsurf, Trae**: Start new chats when switching agents
- **Roo Code**: Switch modes within the same conversation

**Common Task Commands**:

- `*help` - Show available commands
- `*status` - Show current context/progress
- `*exit` - Exit the agent mode
- `*shard-doc docs/prd.md prd` - Shard PRD into manageable pieces
- `*shard-doc docs/architecture.md architecture` - Shard architecture document
- `*create` - Run create-next-story task (SM agent)

**In Web UI**:

```text
/pm create-doc prd
/architect review system design
/dev implement story 1.2
/help - Show available commands
/switch agent-name - Change active agent (if orchestrator available)
```

## Team Configurations

### Pre-Built Teams

#### Team All

- **Includes**: All 10 agents + orchestrator
- **Use Case**: Complete projects requiring all roles
- **Bundle**: `team-all.txt`

#### Team Fullstack

- **Includes**: PM, Architect, Developer, QA, UX Expert
- **Use Case**: End-to-end web/mobile development
- **Bundle**: `team-fullstack.txt`

#### Team No-UI

- **Includes**: PM, Architect, Developer, QA (no UX Expert)
- **Use Case**: Backend services, APIs, system development
- **Bundle**: `team-no-ui.txt`

## Core Architecture

### System Overview

The BMAD-METHOD™ is built around a modular architecture centered on the `bmad-core` directory, which serves as the brain of the entire system. This design enables the framework to operate effectively in both IDE environments (like Cursor, VS Code) and web-based AI interfaces (like ChatGPT, Gemini).

### Key Architectural Components

#### 1. Agents (`bmad-core/agents/`)

- **Purpose**: Each markdown file defines a specialized AI agent for a specific Agile role (PM, Dev, Architect, etc.)
- **Structure**: Contains YAML headers specifying the agent's persona, capabilities, and dependencies
- **Dependencies**: Lists of tasks, templates, checklists, and data files the agent can use
- **Startup Instructions**: Can load project-specific documentation for immediate context

#### 2. Agent Teams (`bmad-core/agent-teams/`)

- **Purpose**: Define collections of agents bundled together for specific purposes
- **Examples**: `team-all.yaml` (comprehensive bundle), `team-fullstack.yaml` (full-stack development)
- **Usage**: Creates pre-packaged contexts for web UI environments

#### 3. Workflows (`bmad-core/workflows/`)

- **Purpose**: YAML files defining prescribed sequences of steps for specific project types
- **Types**: Greenfield (new projects) and Brownfield (existing projects) for UI, service, and fullstack development
- **Structure**: Defines agent interactions, artifacts created, and transition conditions

#### 4. Reusable Resources

- **Templates** (`bmad-core/templates/`): Markdown templates for PRDs, architecture specs, user stories
- **Tasks** (`bmad-core/tasks/`): Instructions for specific repeatable actions like "shard-doc" or "create-next-story"
- **Checklists** (`bmad-core/checklists/`): Quality assurance checklists for validation and review
- **Data** (`bmad-core/data/`): Core knowledge base and technical preferences

### Dual Environment Architecture

#### IDE Environment

- Users interact directly with agent markdown files
- Agents can access all dependencies dynamically
- Supports real-time file operations and project integration
- Optimized for development workflow execution

#### Web UI Environment

- Uses pre-built bundles from `dist/teams` for stand alone 1 upload files for all agents and their assets with an orchestrating agent
- Single text files containing all agent dependencies are in `dist/agents/` - these are unnecessary unless you want to create a web agent that is only a single agent and not a team
- Created by the web-builder tool for upload to web interfaces
- Provides complete context in one package

### Template Processing System

BMad employs a sophisticated template system with three key components:

1. **Template Format** (`utils/bmad-doc-template.md`): Defines markup language for variable substitution and AI processing directives from yaml templates
2. **Document Creation** (`tasks/create-doc.md`): Orchestrates template selection and user interaction to transform yaml spec to final markdown output
3. **Advanced Elicitation** (`tasks/advanced-elicitation.md`): Provides interactive refinement through structured brainstorming

### Technical Preferences Integration

The `technical-preferences.md` file serves as a persistent technical profile that:

- Ensures consistency across all agents and projects
- Eliminates repetitive technology specification
- Provides personalized recommendations aligned with user preferences
- Evolves over time with lessons learned

### Build and Delivery Process

The `web-builder.js` tool creates web-ready bundles by:

1. Reading agent or team definition files
2. Recursively resolving all dependencies
3. Concatenating content into single text files with clear separators
4. Outputting ready-to-upload bundles for web AI interfaces

This architecture enables seamless operation across environments while maintaining the rich, interconnected agent ecosystem that makes BMad powerful.

## Complete Development Workflow

### Planning Phase (Web UI Recommended - Especially Gemini!)

**Ideal for cost efficiency with Gemini's massive context:**

**For Brownfield Projects - Start Here!**:

1. **Upload entire project to Gemini Web** (GitHub URL, files, or zip)
2. **Document existing system**: `/analyst` → `*document-project`
3. **Creates comprehensive docs** from entire codebase analysis

**For All Projects**:

1. **Optional Analysis**: `/analyst` - Market research, competitive analysis
2. **Project Brief**: Create foundation document (Analyst or user)
3. **PRD Creation**: `/pm create-doc prd` - Comprehensive product requirements
4. **Architecture Design**: `/architect create-doc architecture` - Technical foundation
5. **Validation & Alignment**: `/po` run master checklist to ensure document consistency
6. **Document Preparation**: Copy final documents to project as `docs/prd.md` and `docs/architecture.md`

#### Example Planning Prompts

**For PRD Creation**:

```text
"I want to build a [type] application that [core purpose].
Help me brainstorm features and create a comprehensive PRD."
```

**For Architecture Design**:

```text
"Based on this PRD, design a scalable technical architecture
that can handle [specific requirements]."
```

### Critical Transition: Web UI to IDE

**Once planning is complete, you MUST switch to IDE for development:**

- **Why**: Development workflow requires file operations, real-time project integration, and document sharding
- **Cost Benefit**: Web UI is more cost-effective for large document creation; IDE is optimized for development tasks
- **Required Files**: Ensure `docs/prd.md` and `docs/architecture.md` exist in your project

### IDE Development Workflow

**Prerequisites**: Planning documents must exist in `docs/` folder

1. **Document Sharding** (CRITICAL STEP):
   - Documents created by PM/Architect (in Web or IDE) MUST be sharded for development
   - Two methods to shard:
     a) **Manual**: Drag `shard-doc` task + document file into chat
     b) **Agent**: Ask `@bmad-master` or `@po` to shard documents
   - Shards `docs/prd.md` → `docs/prd/` folder
   - Shards `docs/architecture.md` → `docs/architecture/` folder
   - **WARNING**: Do NOT shard in Web UI - copying many small files is painful!

2. **Verify Sharded Content**:
   - At least one `epic-n.md` file in `docs/prd/` with stories in development order
   - Source tree document and coding standards for dev agent reference
   - Sharded docs for SM agent story creation

Resulting Folder Structure:

- `docs/prd/` - Broken down PRD sections
- `docs/architecture/` - Broken down architecture sections
- `docs/stories/` - Generated user stories

1. **Development Cycle** (Sequential, one story at a time):

   **CRITICAL CONTEXT MANAGEMENT**:
   - **Context windows matter!** Always use fresh, clean context windows
   - **Model selection matters!** Use most powerful thinking model for SM story creation
   - **ALWAYS start new chat between SM, Dev, and QA work**

   **Step 1 - Story Creation**:
   - **NEW CLEAN CHAT** → Select powerful model → `@sm` → `*create`
   - SM executes create-next-story task
   - Review generated story in `docs/stories/`
   - Update status from "Draft" to "Approved"

   **Step 2 - Story Implementation**:
   - **NEW CLEAN CHAT** → `@dev`
   - Agent asks which story to implement
   - Include story file content to save dev agent lookup time
   - Dev follows tasks/subtasks, marking completion
   - Dev maintains File List of all changes
   - Dev marks story as "Review" when complete with all tests passing

   **Step 3 - Senior QA Review**:
   - **NEW CLEAN CHAT** → `@qa` → execute review-story task
   - QA performs senior developer code review
   - QA can refactor and improve code directly
   - QA appends results to story's QA Results section
   - If approved: Status → "Done"
   - If changes needed: Status stays "Review" with unchecked items for dev

   **Step 4 - Repeat**: Continue SM → Dev → QA cycle until all epic stories complete

**Important**: Only 1 story in progress at a time, worked sequentially until all epic stories complete.

### Status Tracking Workflow

Stories progress through defined statuses:

- **Draft** → **Approved** → **InProgress** → **Done**

Each status change requires user verification and approval before proceeding.

### Workflow Types

#### Greenfield Development

- Business analysis and market research
- Product requirements and feature definition
- System architecture and design
- Development execution
- Testing and deployment

#### Brownfield Enhancement (Existing Projects)

**Key Concept**: Brownfield development requires comprehensive documentation of your existing project for AI agents to understand context, patterns, and constraints.

**Complete Brownfield Workflow Options**:

**Option 1: PRD-First (Recommended for Large Codebases/Monorepos)**:

1. **Upload project to Gemini Web** (GitHub URL, files, or zip)
2. **Create PRD first**: `@pm` → `*create-doc brownfield-prd`
3. **Focused documentation**: `@analyst` → `*document-project`
   - Analyst asks for focus if no PRD provided
   - Choose "single document" format for Web UI
   - Uses PRD to document ONLY relevant areas
   - Creates one comprehensive markdown file
   - Avoids bloating docs with unused code

**Option 2: Document-First (Good for Smaller Projects)**:

1. **Upload project to Gemini Web**
2. **Document everything**: `@analyst` → `*document-project`
3. **Then create PRD**: `@pm` → `*create-doc brownfield-prd`
   - More thorough but can create excessive documentation

4. **Requirements Gathering**:
   - **Brownfield PRD**: Use PM agent with `brownfield-prd-tmpl`
   - **Analyzes**: Existing system, constraints, integration points
   - **Defines**: Enhancement scope, compatibility requirements, risk assessment
   - **Creates**: Epic and story structure for changes

5. **Architecture Planning**:
   - **Brownfield Architecture**: Use Architect agent with `brownfield-architecture-tmpl`
   - **Integration Strategy**: How new features integrate with existing system
   - **Migration Planning**: Gradual rollout and backwards compatibility
   - **Risk Mitigation**: Addressing potential breaking changes

**Brownfield-Specific Resources**:

**Templates**:

- `brownfield-prd-tmpl.md`: Comprehensive enhancement planning with existing system analysis
- `brownfield-architecture-tmpl.md`: Integration-focused architecture for existing systems

**Tasks**:

- `document-project`: Generates comprehensive documentation from existing codebase
- `brownfield-create-epic`: Creates single epic for focused enhancements (when full PRD is overkill)
- `brownfield-create-story`: Creates individual story for small, isolated changes

**When to Use Each Approach**:

**Full Brownfield Workflow** (Recommended for):

- Major feature additions
- System modernization
- Complex integrations
- Multiple related changes

**Quick Epic/Story Creation** (Use when):

- Single, focused enhancement
- Isolated bug fixes
- Small feature additions
- Well-documented existing system

**Critical Success Factors**:

1. **Documentation First**: Always run `document-project` if docs are outdated/missing
2. **Context Matters**: Provide agents access to relevant code sections
3. **Integration Focus**: Emphasize compatibility and non-breaking changes
4. **Incremental Approach**: Plan for gradual rollout and testing

**For detailed guide**: See `docs/working-in-the-brownfield.md`

## Document Creation Best Practices

### Required File Naming for Framework Integration

- `docs/prd.md` - Product Requirements Document
- `docs/architecture.md` - System Architecture Document

**Why These Names Matter**:

- Agents automatically reference these files during development
- Sharding tasks expect these specific filenames
- Workflow automation depends on standard naming

### Cost-Effective Document Creation Workflow

**Recommended for Large Documents (PRD, Architecture):**

1. **Use Web UI**: Create documents in web interface for cost efficiency
2. **Copy Final Output**: Save complete markdown to your project
3. **Standard Names**: Save as `docs/prd.md` and `docs/architecture.md`
4. **Switch to IDE**: Use IDE agents for development and smaller documents

### Document Sharding

Templates with Level 2 headings (`##`) can be automatically sharded:

**Original PRD**:

```markdown
## Goals and Background Context

## Requirements

## User Interface Design Goals

## Success Metrics
```

**After Sharding**:

- `docs/prd/goals-and-background-context.md`
- `docs/prd/requirements.md`
- `docs/prd/user-interface-design-goals.md`
- `docs/prd/success-metrics.md`

Use the `shard-doc` task or `@kayvan/markdown-tree-parser` tool for automatic sharding.

## Usage Patterns and Best Practices

### Environment-Specific Usage

**Web UI Best For**:

- Initial planning and documentation phases
- Cost-effective large document creation
- Agent consultation and brainstorming
- Multi-agent workflows with orchestrator

**IDE Best For**:

- Active development and implementation
- File operations and project integration
- Story management and development cycles
- Code review and debugging

### Quality Assurance

- Use appropriate agents for specialized tasks
- Follow Agile ceremonies and review processes
- Maintain document consistency with PO agent
- Regular validation with checklists and templates

### Performance Optimization

- Use specific agents vs. `bmad-master` for focused tasks
- Choose appropriate team size for project needs
- Leverage technical preferences for consistency
- Regular context management and cache clearing

## Success Tips

- **Use Gemini for big picture planning** - The team-fullstack bundle provides collaborative expertise
- **Use bmad-master for document organization** - Sharding creates manageable chunks
- **Follow the SM → Dev cycle religiously** - This ensures systematic progress
- **Keep conversations focused** - One agent, one task per conversation
- **Review everything** - Always review and approve before marking complete

## Contributing to BMAD-METHOD™

### Quick Contribution Guidelines

For full details, see `CONTRIBUTING.md`. Key points:

**Fork Workflow**:

1. Fork the repository
2. Create feature branches
3. Submit PRs to `next` branch (default) or `main` for critical fixes only
4. Keep PRs small: 200-400 lines ideal, 800 lines maximum
5. One feature/fix per PR

**PR Requirements**:

- Clear descriptions (max 200 words) with What/Why/How/Testing
- Use conventional commits (feat:, fix:, docs:)
- Atomic commits - one logical change per commit
- Must align with guiding principles

**Core Principles** (from docs/GUIDING-PRINCIPLES.md):

- **Dev Agents Must Be Lean**: Minimize dependencies, save context for code
- **Natural Language First**: Everything in markdown, no code in core
- **Core vs Expansion Packs**: Core for universal needs, packs for specialized domains
- **Design Philosophy**: "Dev agents code, planning agents plan"

## Expansion Packs

### What Are Expansion Packs?

Expansion packs extend BMAD-METHOD™ beyond traditional software development into ANY domain. They provide specialized agent teams, templates, and workflows while keeping the core framework lean and focused on development.

### Why Use Expansion Packs?

1. **Keep Core Lean**: Dev agents maintain maximum context for coding
2. **Domain Expertise**: Deep, specialized knowledge without bloating core
3. **Community Innovation**: Anyone can create and share packs
4. **Modular Design**: Install only what you need

### Available Expansion Packs

**Technical Packs**:

- **Infrastructure/DevOps**: Cloud architects, SRE experts, security specialists
- **Game Development**: Game designers, level designers, narrative writers
- **Mobile Development**: iOS/Android specialists, mobile UX experts
- **Data Science**: ML engineers, data scientists, visualization experts

**Non-Technical Packs**:

- **Business Strategy**: Consultants, financial analysts, marketing strategists
- **Creative Writing**: Plot architects, character developers, world builders
- **Health & Wellness**: Fitness trainers, nutritionists, habit engineers
- **Education**: Curriculum designers, assessment specialists
- **Legal Support**: Contract analysts, compliance checkers

**Specialty Packs**:

- **Expansion Creator**: Tools to build your own expansion packs
- **RPG Game Master**: Tabletop gaming assistance
- **Life Event Planning**: Wedding planners, event coordinators
- **Scientific Research**: Literature reviewers, methodology designers

### Using Expansion Packs

1. **Browse Available Packs**: Check `expansion-packs/` directory
2. **Get Inspiration**: See `docs/expansion-packs.md` for detailed examples and ideas
3. **Install via CLI**:

   ```bash
   npx bmad-method install
   # Select "Install expansion pack" option
   ```

4. **Use in Your Workflow**: Installed packs integrate seamlessly with existing agents

### Creating Custom Expansion Packs

Use the **expansion-creator** pack to build your own:

1. **Define Domain**: What expertise are you capturing?
2. **Design Agents**: Create specialized roles with clear boundaries
3. **Build Resources**: Tasks, templates, checklists for your domain
4. **Test & Share**: Validate with real use cases, share with community

**Key Principle**: Expansion packs democratize expertise by making specialized knowledge accessible through AI agents.

## Getting Help

- **Commands**: Use `*/*help` in any environment to see available commands
- **Agent Switching**: Use `*/*switch agent-name` with orchestrator for role changes
- **Documentation**: Check `docs/` folder for project-specific context
- **Community**: Discord and GitHub resources available for support
- **Contributing**: See `CONTRIBUTING.md` for full guidelines
