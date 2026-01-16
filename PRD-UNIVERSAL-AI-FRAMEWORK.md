# Product Requirements Document (PRD)
## Universal AI Framework

**Version:** 1.0.0
**Status:** Draft
**Last Updated:** 2025-01-15
**Product Owner:** Galando
**Repository:** [universal-ai-framework](https://github.com/galando/universal-ai-framework)
**Parent Repository:** [claude-piv-skeleton](https://github.com/galando/claude-piv-skeleton)

---

## 1. Executive Summary

**Universal AI Framework** is a complete, professional development framework that transforms any AI coding assistant (Claude Code, Cursor, GitHub Copilot, OpenAI Codex) into a production-ready development partner. It enforces strict Test-Driven Development (TDD), provides automatic validation, creates workflow artifacts, and maintains consistent quality standards across all AI tools.

This is a **new repository** forked from `claude-piv-skeleton`, transforming it from a Claude-specific tool into a universal framework that works with any AI assistant while preserving and enhancing all existing functionality.

**Core Value Proposition:**
- **Universal Compatibility**: Identical professional workflow across Claude, Cursor, Copilot, Codex, or any AI tool
- **Zero Vendor Lock-in**: Switch between AI tools without relearning workflows
- **Strict Quality Enforcement**: Mandatory TDD, automatic validation, comprehensive rules
- **Complete Workflow System**: Prime (context) → Plan (design) → Implement (TDD) → Validate (quality)
- **Professional Artifacts**: Context documents, implementation plans, validation reports, code reviews

**MVP Goal:**
Create a universal framework that provides complete feature parity across all major AI coding tools, with professional-grade automation, enforcement, and artifact generation - making "ship production-ready code with any AI tool" a reality.

---

## 2. Mission

### Mission Statement
> "To professionalize AI-assisted software development by providing a universal framework that enforces strict quality standards, automatic validation, and consistent workflows across all AI coding assistants."

### Core Principles

1. **Universality First** - The framework must work identically across all AI tools, regardless of vendor or capabilities
2. **Quality Non-Negotiable** - Strict TDD, validation, and code review are mandatory, not optional
3. **Automation Everywhere** - Skills, validation, and artifact creation happen automatically via each tool's native systems
4. **Developer Empowerment** - Clear commands, predictable behavior, and consistent documentation enable developers to focus on building
5. **Community-Driven** - Open, extensible architecture allowing contributions for new tools, technologies, and practices
6. **Production-Ready** - Every feature is designed for real-world production use, not demos or experiments

---

## 3. Target Users

### Primary User Personas

#### Persona 1: The AI-Native Full-Stack Developer

**Profile:** Senior developer using AI assistants daily for production work
**Technical Comfort:** High - comfortable with CLI, git, multiple AI tools, TDD
**Key Needs:**
- Consistent professional workflow across Claude, Cursor, Copilot, Codex
- Strict TDD enforcement (no skipping, no exceptions)
- Automatic validation and quality gates
- Artifact generation for team visibility
- Zero friction when switching between tools

**Pain Points:**
- Each AI tool has different workflows and commands
- Quality varies wildly (no TDD enforcement in most tools)
- Hard to maintain standards when using multiple tools
- No unified artifact/review system
- Tool-specific knowledge doesn't transfer

**Why Universal AI Framework:**
- Same commands (`/prime`, `/execute`, `/validate`) work everywhere
- Automatic TDD enforcement via native skill systems
- Consistent artifacts and validation reports
- Switch tools without losing productivity

---

#### Persona 2: The Engineering Manager / Team Lead

**Profile:** Technical leader managing 5-20 developers using various AI tools
**Technical Comfort:** Medium to High
**Key Needs:**
- Consistent quality standards across team using different AI tools
- Enforced TDD and validation (team can't skip)
- Visibility into development process (artifacts, reports)
- Easy onboarding for new team members
- Audit trail of AI-assisted development

**Pain Points:**
- Team uses Claude, Cursor, Copilot inconsistently
- No unified quality enforcement
- Hard to review AI-generated code across tools
- No visibility into what AI did (no artifacts)
- Onboarding each tool is time-consuming

**Why Universal AI Framework:**
- Same standards and workflow regardless of AI tool choice
- Automatic quality enforcement (can't be disabled)
- Artifacts provide audit trail and visibility
- One onboarding process works for all tools

---

#### Persona 3: The Cursor/Copilot Power User

**Profile:** Developer using Cursor or GitHub Copilot (not Claude Code)
**Technical Comfort:** Medium to High
**Key Needs:**
- Professional workflow for their preferred AI tool
- Access to TDD enforcement and validation
- Clear documentation and examples
- Easy setup and installation
- Feature parity with Claude Code users

**Pain Points:**
- Most "AI workflow" tools are Claude-specific
- No structured methodology for Cursor/Copilot
- Must manually enforce TDD and quality
- Missing professional-grade tooling
- Feel like "second-class citizen" to Claude users

**Why Universal AI Framework:**
- First-class support for Cursor, Copilot, Codex
- Same professional features as Claude Code
- Native skill implementations for each tool
- Clear setup guides for each tool

---

#### Persona 4: The Agency / Consultancy Developer

**Profile:** Developer at agency working with multiple clients and tech stacks
**Technical Comfort:** High
**Key Needs:**
- Universal workflow that works across client projects
- Technology-agnostic (Spring Boot, Node, React, all supported)
- Professional quality standards clients expect
- Easy to install and configure in new projects
- Artifact trail for client deliverables

**Pain Points:**
- Different clients prefer different AI tools
- Need consistent quality across all projects
- Hard to maintain standards across diverse tech stacks
- Training overhead for each new tool/stack
- Clients want visibility into AI usage

**Why Universal AI Framework:**
- Works with any AI tool client prefers
- Technology templates for all major stacks
- Artifacts provide deliverable documentation
- Same workflow regardless of tech stack

---

### Secondary Users

#### Persona 5: The Open Source Contributor

**Profile:** Developer contributing to open source using AI tools
**Needs:**
- Clear contribution standards
- Consistent workflow across projects
- Easy to add new technology templates
- Community-driven extension points

#### Persona 6: The Startup CTO

**Profile:** Technical founder building team and processes
**Needs:**
- Scalable development practices
- Quality standards from day one
- Team onboarding streamlined
- Professional practices investors expect

---

## 4. MVP Scope

### What Is This Project?

**Universal AI Framework** is a **new repository** that will be forked from `claude-piv-skeleton` and transformed into a universal framework. The original `claude-piv-skeleton` repository will remain unchanged and continue to serve Claude Code users who prefer a Claude-focused workflow.

**Relationship:**
```
claude-piv-skeleton (existing)
├── Claude-focused
├── Proven, stable
└── Continues for Claude-only users

universal-ai-framework (new)
├── Forked from claude-piv-skeleton
├── Enhanced for universal compatibility
├── Supports: Claude, Cursor, Copilot, Codex
└── Future: More AI tools
```

---

### ✅ In Scope for MVP

#### Universal Core (All AI Tools)

**Directory Structure:**
- [x] `.ai-universal/` - Universal core framework
- [x] `.ai-commands/` - Universal command system
- [x] `.ai-universal/skills/` - Universal skill definitions
- [x] `.ai-universal/rules/` - Universal rules (TDD, Git, Testing, etc.)
- [x] `.ai-universal/artifacts/` - Universal artifact structure
- [x] `.ai-universal/methodology/` - PIV methodology docs
- [x] `.ai-universal/prompts/` - Universal prompt library

**Core Features:**
- [x] Universal command system (`/prime`, `/plan`, `/execute`, `/validate`, `/commit`, `/review`)
- [x] Universal prompt library that works with any AI tool
- [x] Universal rules extracted from `.claude/rules/`
- [x] Universal skill definitions (tool-agnostic)
- [x] Universal artifact system (context, plans, reports, reviews)
- [x] PIV methodology documentation (tool-agnostic)
- [x] Technology templates (Spring Boot, Node, React, PostgreSQL, Docker)
- [x] Prompt library for manual AI tools (ChatGPT, etc.)

---

#### Tool-Specific Implementations

**Claude Code (Enhanced - Feature Parity):**
- [x] `.claude/` directory (all existing functionality)
- [x] Native commands (`/piv_loop:*`, `/validation:*`, `/bug_fix:*`, `/product:create-prd`)
- [x] Auto-activating skills (TDD, code review, validation)
- [x] Agent orchestration
- [x] Artifact auto-generation
- [x] **No regression** - all features work exactly as before

**Cursor (First-Class Support):**
- [x] `.cursor/` directory structure
- [x] `.cursorrules` with universal command routing
- [x] Cursor-specific skill implementations (rules engine)
- [x] Text expansion snippets (workflow shortcuts)
- [x] Setup guide for Cursor users

**GitHub Copilot (First-Class Support):**
- [x] `.github/` directory
- [x] `copilot-instructions.md` with universal prompts
- [x] Copilot Workspace integration
- [x] Copilot-specific skill implementations
- [x] Setup guide for Copilot users

**OpenAI Codex (First-Class Support):**
- [x] `.openai/` directory structure
- [x] Codex instructions with universal prompts
- [x] Codex-specific skill implementations
- [x] Setup guide for Codex users

---

#### Complete Feature Set (From claude-piv-skeleton)

**PIV Methodology:**
- [x] **Prime Phase** - Context loading and understanding
- [x] **Plan Phase** - Detailed implementation planning
- [x] **Implement Phase** - TDD-driven execution (RED-GREEN-REFACTOR)
- [x] **Validate Phase** - Comprehensive validation pipeline
- [x] Phase-based commits (one commit per phase)

**Command Infrastructure (All Tools):**
- [x] `/prime` - Load codebase context
- [x] `/plan <feature>` - Create implementation plan
- [x] `/execute [plan]` - Execute with TDD enforcement
- [x] `/validate` - Quick validation
- [x] `/validate:full` - Comprehensive validation pipeline
- [x] `/review` - Technical code review
- [x] `/review:fix` - Fix code review issues
- [x] `/report:execution` - Execution report
- [x] `/report:system` - Process improvement analysis
- [x] `/commit` - Conventional commits (delegates to commit-commands plugin)
- [x] `/rca` - Root cause analysis for bugs
- [x] `/fix` - Implement bug fix from RCA
- [x] `/prd` - Create Product Requirements Document

**Claude Code Commands (Preserved):**
- [x] `/piv_loop:prime` - Prime workspace
- [x] `/piv_loop:plan-feature` - Create feature plan
- [x] `/piv_loop:execute` - Execute plan
- [x] `/validation:validate` - Full validation pipeline
- [x] `/validation:code-review` - Technical code review
- [x] `/validation:code-review-fix` - Fix review issues
- [x] `/validation:execution-report` - Execution report
- [x] `/validation:system-review` - System review
- [x] `/bug_fix:rca` - Root cause analysis
- [x] `/bug_fix:implement-fix` - Implement fix
- [x] `/product:create-prd` - Create PRD

---

#### Skills System (Universal + Tool-Specific)

**Universal Skill Definitions:**
- [x] `tdd-enforcement` - Enforce RED-GREEN-REFACTOR cycle
- [x] `test-writing` - Given-When-Then structure
- [x] `auto-validation` - Automatic validation after execute
- [x] `artifact-creation` - Automatic artifact generation
- [x] `conventional-commit` - Enforce commit message format
- [x] `code-review` - Technical review
- [x] `api-design` - REST API best practices
- [x] `security` - Security guidelines

**Tool Implementations:**
- [x] Claude: Native skills (`.claude/skills/`)
- [x] Cursor: Rules engine (`.cursor/rules/`)
- [x] Copilot: Instructions system (`.github/copilot-skills/`)
- [x] Codex: Custom system (`.openai/skills/`)

---

#### Rules System (Complete)

**Universal Rules:**
- [x] `00-general.md` - Core development principles
- [x] `10-git.md` - Git workflow + phase-based commits + main branch protection
- [x] `20-testing.md` - Testing philosophy
- [x] `21-testing.md` - Given-When-Then structure
- [x] `22-tdd-strict.md` - **MANDATORY** TDD enforcement
- [x] `30-documentation.md` - Documentation standards
- [x] `40-security.md` - Security best practices

**Technology-Specific Rules:**
- [x] `backend/10-api-design.md` - REST API patterns
- [x] `backend/20-database.md` - Database patterns

---

#### Validation System (Complete)

**Validation Pipeline:**
- [x] Environment safety check (DEV/TEST vs PROD detection)
- [x] Build verification
- [x] Unit tests
- [x] Integration tests
- [x] E2E tests (if exist)
- [x] Code quality analysis
- [x] Coverage analysis (≥80% target)
- [x] Security scanning (SQL injection, XSS, sensitive data)
- [x] Dependency auditing
- [x] **TDD compliance check** (tests written before code)
- [x] **Pragmatic Programmer principles** check
- [x] Rule compliance verification
- [x] Validation report generation

---

#### Artifact System (Complete)

**Artifact Types:**
- [x] **Context Artifacts** (`.ai-universal/artifacts/context/`)
  - Prime-phase context documents
  - Codebase summaries
  - Architecture overviews
  - Pattern inventories

- [x] **Plan Artifacts** (`.ai-universal/artifacts/plans/`)
  - Implementation plans
  - Step-by-step guides
  - Risk assessments
  - Approval checklists

- [x] **Validation Reports** (`.ai-universal/artifacts/reports/`)
  - Full validation results
  - Test coverage analysis
  - Quality metrics
  - Issue lists

- [x] **Execution Reports** (`.ai-universal/artifacts/reports/`)
  - Implementation summaries
  - Files changed
  - Tests added
  - Validation results

- [x] **System Reviews** (`.ai-universal/artifacts/reports/`)
  - Plan vs actual analysis
  - Process improvements
  - Lessons learned

- [x] **Code Reviews** (`.ai-universal/artifacts/reviews/`)
  - Technical quality assessments
  - Issue lists
  - Fix recommendations

- [x] **RCA Reports** (`.ai-universal/artifacts/reviews/`)
  - Root cause analysis
  - Bug descriptions
  - Fix approaches

---

#### Agent System (Universal)

**Agent Definitions:**
- [x] **Context Agent** (Prime phase) - Load codebase understanding
- [x] **Planning Agent** (Plan phase) - Create detailed plans
- [x] **Implementation Agent** (Implement phase) - Execute with TDD
- [x] **Validation Agent** (Validate phase) - Verify quality
- [x] **Review Agent** - Code quality checks

**Universal Agent Concept:**
- [x] `docs/AGENTS.md` - Universal agent documentation
- [x] Agent artifact templates
- [x] Tool-specific agent implementations

---

#### Git Workflow Features

**Complete Git Integration:**
- [x] **Conventional commits** - Standardized format
- [x] **Main branch protection** - No direct commits to main
- [x] **Feature branch workflow** - All changes via PR
- [x] **Phase-based commits** - One commit per PIV phase
- [x] **Atomic commits** - Small, focused changes
- [x] **Commit message generator** - Auto-generate from changes
- [x] **Commit hooks** - Enforce standards (future)

---

#### Technology Templates

**All Existing Templates Preserved:**
- [x] **Backend**: Spring Boot, Node.js/Express, Python/FastAPI
- [x] **Frontend**: React with TypeScript
- [x] **Database**: PostgreSQL
- [x] **DevOps**: Docker

**Each Template Includes:**
- [x] Technology-specific rules
- [x] Best practices reference
- [x] Code examples
- [x] Integration guides
- [x] README documentation

---

#### Documentation & Onboarding

**Complete Documentation:**
- [x] **Landing Page** (`docs/index.md`) - GitHub Pages site
- [x] **Universal Command Reference** (`.ai-commands/COMMANDS.md`)
- [x] **Universal Agent Documentation** (`docs/AGENTS.md`)
- [x] **Methodology Guide** (`docs/METHODOLOGY.md`)
- [x] **Skill System Documentation** (`docs/skills/`)
- [x] **Getting Started Guides**:
  - [x] Installation guide
  - [x] Quick start (5 minutes)
  - [x] Your first feature
  - [x] Tool-specific guides:
    - [x] Claude Code
    - [x] Cursor
    - [x] GitHub Copilot
    - [x] OpenAI Codex
- [x] **Extending Framework**:
  - [x] Adding new technologies
  - [x] Adding new AI tools
  - [x] Creating custom skills
  - [x] Creating custom rules
- [x] **Troubleshooting Guide**
- [x] **FAQ**
- [x] **Migration Guide** (from claude-piv-skeleton)

---

#### Installation & Setup

**Installation System:**
- [x] **One-line install** (curl script)
- [x] **Fork and clone** instructions
- [x] **Setup wizard** (interactive script)
- [x] **Technology auto-detection** (Spring Boot, Node, React, etc.)
- [x] **Tool detection** (Claude, Cursor, Copilot, Codex)
- [x] **Backup before install** (safety)
- [x] **Verification tests** (post-install validation)

---

### ❌ Out of Scope for MVP

**Future Enhancements (Post-MVP):**
- [ ] Web-based UI for configuration
- [ ] Interactive setup wizard (GUI)
- [ ] Pre-built integrations for other AI tools (Tabnine, CodeWhisperer, etc.)
- [ ] Cloud-hosted artifact storage
- [ ] Team analytics and reporting dashboard
- [ ] IDE extensions (VS Code, JetBrains)
- [ ] CI/CD integration (GitHub Actions validation)
- [ ] Automatic technology detection (enhanced)
- [ ] Custom command builder (GUI)
- [ ] Plugin system for extending functionality
- [ ] Remote execution support
- [ ] Artifact versioning and history
- [ ] Team collaboration features (sharing artifacts)
- [ ] Multi-agent collaboration (agents talking to agents)

**Advanced Features (v3.0+):**
- [ ] Learning from user patterns
- [ ] Predictive validation
- [ ] Intelligent test generation
- [ ] Custom rule builder (GUI)
- [ ] SSO integration
- [ ] Audit logging
- [ ] Compliance reporting
- [ ] On-premise deployment
- [ ] Enterprise features

---

## 5. User Stories

### Primary User Stories

#### Story 1: Universal Command Execution

**As a** developer using multiple AI tools
**I want to** type `/prime`, `/execute`, `/validate` and have them work identically in Claude, Cursor, Copilot, and Codex
**So that** I can switch between tools without relearning workflows or losing productivity

**Acceptance Criteria:**
- [x] `/prime` loads context in all 4 tools (same artifact structure)
- [x] `/execute` follows TDD cycle in all 4 tools
- [x] `/validate:full` runs same validation checks in all 4 tools
- [x] Artifact structure identical across all tools
- [x] Error messages consistent across all tools

**Example:**
```bash
# Morning: Using Claude Code
User: /prime
Claude: ✓ Context loaded: Spring Boot project, 12 modules
Claude: Artifact: .ai-universal/artifacts/context/prime-2025-01-15.md

# Afternoon: Switch to Cursor
User: /prime
Cursor: ✓ Context loaded: Spring Boot project, 12 modules
Cursor: Artifact: .ai-universal/artifacts/context/prime-2025-01-15.md

# Result: Same artifact, same information, different tool
```

---

#### Story 2: Automatic TDD Enforcement

**As a** developer using any AI tool
**I want** TDD enforcement to happen automatically (not manually)
**So that** I never skip TDD or write code before tests

**Acceptance Criteria:**
- [x] TDD skill auto-activates in Claude Code (existing)
- [x] TDD rule auto-activates in Cursor (new)
- [x] TDD instruction auto-activates in Copilot (new)
- [x] TDD skill auto-activates in Codex (new)
- [x] Enforcement is strict (deletes code if TDD violated)
- [x] Error message consistent: "Write test first (RED phase)"

**Example:**
```bash
# Claude Code
User: [Starts writing implementation code]
Claude Skill: [Auto-activates] "Test file missing. Write test first (RED phase)"
Claude: [Deletes implementation code]

# Cursor (same behavior)
User: [Starts writing implementation code]
Cursor Rule: [Auto-activates] "Test file missing. Write test first (RED phase)"
Cursor: [Deletes implementation code]

# Result: Same enforcement, different tool mechanism
```

---

#### Story 3: Automatic Validation After Execution

**As a** developer
**I want** validation to run automatically after `/execute` completes
**So that** I don't forget to validate or ship broken code

**Acceptance Criteria:**
- [x] Validation auto-activates after `/execute` in Claude Code (existing)
- [x] Validation auto-activates after `/execute` in Cursor (new)
- [x] Validation auto-activates after `/execute` in Copilot (new)
- [x] Validation auto-activates after `/execute` in Codex (new)
- [x] Validation report created automatically
- [x] Results displayed consistently

**Example:**
```bash
# Claude Code
User: /execute auth-plan
Claude: [Executes plan with TDD]
Claude: [Auto-validates] ✓ Tests: 47/47, Coverage: 89%
Claude: Report: .ai-universal/artifacts/reports/validation-2025-01-15.md

# Cursor (same flow)
User: /execute auth-plan
Cursor: [Executes plan with TDD]
Cursor: [Auto-validates] ✓ Tests: 47/47, Coverage: 89%
Cursor: Report: .ai-universal/artifacts/reports/validation-2025-01-15.md

# Result: Same automatic validation, same report
```

---

#### Story 4: Artifact Visibility for Teams

**As a** team lead
**I want to** see all artifacts created by my team (context, plans, reports)
**So that** I can understand the development process and review AI-assisted work

**Acceptance Criteria:**
- [x] All artifacts stored in `.ai-universal/artifacts/`
- [x] Artifact structure consistent across all tools
- [x] Artifact naming includes timestamp and type
- [x] Artifacts are markdown (readable in git)
- [x] Artifacts committed to git (audit trail)
- [x] Team can review artifacts in PRs

**Example:**
```
.ai-universal/artifacts/
├── context/
│   └── prime-2025-01-15.md              # Context loaded
├── plans/
│   ├── auth-jwt-plan.md                 # Implementation plan
│   └── user-profile-plan.md             # Another plan
├── reports/
│   ├── validation-2025-01-15.md         # Validation after execute
│   ├── execution-auth-jwt.md            # Execution summary
│   └── system-review-auth-jwt.md        # Process analysis
└── reviews/
    ├── code-review-2025-01-15.md        # Technical review
    └── rca-issue-123.md                 # Bug analysis

# Team lead can review all artifacts in git/PR
```

---

#### Story 5: Complete Feature Parity

**As a** Cursor user
**I want** access to all the same features as Claude Code users
**So that** I'm not missing out on professional capabilities

**Acceptance Criteria:**
- [x] All commands work (`/prime`, `/plan`, `/execute`, `/validate`, `/commit`, `/review`)
- [x] All validation checks run (TDD, coverage, security, etc.)
- [x] All artifacts created (context, plans, reports, reviews)
- [x] All skills activate (TDD, validation, artifact creation)
- [x] Quality identical to Claude Code experience
- [x] Documentation specific to Cursor

**Example:**
```bash
# Claude Code user
/prime → /plan → /execute → /validate → /commit
✓ Full professional workflow with automation

# Cursor user
/prime → /plan → /execute → /validate → /commit
✓ Same professional workflow with automation

# Result: No feature gap, equal experience
```

---

#### Story 6: Quick Setup for New Projects

**As a** developer starting a new project
**I want to** run one command and have the framework installed and configured
**So that** I can start coding immediately

**Acceptance Criteria:**
- [x] One-line install command works
- [x] Auto-detects technology stack
- [x] Auto-detects AI tools installed
- [x] Installs appropriate configuration
- [x] Runs verification tests
- [x] Shows quick start next steps

**Example:**
```bash
$ curl -s https://raw.githubusercontent.com/galando/universal-ai-framework/main/install.sh | bash

✓ Universal AI Framework Installer
✓ Detecting project type... Spring Boot (Java 17)
✓ Detecting AI tools... Claude Code, Cursor
✓ Installing universal commands...
✓ Installing Claude skills...
✓ Installing Cursor rules...
✓ Running verification...
✓ All tests passing!

🚀 Ready to code!
Try: /prime   (load context)
     /plan "Add user authentication"
     /execute

Docs: https://universal-ai-framework.dev
```

---

#### Story 7: Bug Fix Workflow

**As a** developer fixing a bug
**I want** to follow a structured bug fix process with RCA and validation
**So that** bugs are fixed correctly and permanently

**Acceptance Criteria:**
- [x] `/rca` performs root cause analysis
- [x] Creates RCA artifact
- [x] `/fix` implements fix with TDD
- [x] Validation runs automatically
- [x] Fix verified before commit

**Example:**
```bash
# Bug report: "Login fails for users with special characters in email"

User: /rca "Login fails for special characters in email"
AI: [Analyzes code, identifies root cause]
AI: RCA Report: .ai-universal/artifacts/reviews/rca-login-2025-01-15.md
AI: Root Cause: Email validation regex doesn't handle special chars
AI: Recommendation: Update regex, add tests for edge cases

User: /fix rca-login-2025-01-15
AI: [Following TDD]
AI: [Test 1/2] Test for special characters → FAILS ✓
AI: [Implement] Fix regex → PASSES ✓
AI: [Test 2/2] Test for valid emails → PASSES ✓
AI: [Auto-validates] ✓ All tests passing
AI: Ready to commit?

User: /commit
AI: feat(auth): fix email validation for special characters
```

---

#### Story 8: Technology Template Usage

**As a** developer starting a Spring Boot project
**I want** to use the Spring Boot template
**So that** I get Spring-specific rules and best practices

**Acceptance Criteria:**
- [x] Technology templates exist for all major stacks
- [x] Each template includes technology-specific rules
- [x] Each template includes best practices reference
- [x] Each template includes code examples
- [x] Templates are easy to use

**Example:**
```bash
# New Spring Boot project

User: [Uses Spring Boot template]
Installed:
✓ technologies/backend/spring-boot/rules/api-design.md
✓ technologies/backend/spring-boot/rules/database.md
✓ technologies/backend/spring-boot/reference/spring-boot-best-practices.md
✓ technologies/backend/spring-boot/examples/

Now when I develop:
✓ Spring-specific rules auto-load
✓ Spring best practices apply
✓ Spring code examples available
```

---

### Technical User Stories

#### Story 9: Universal Skill Definition

**As a** framework developer
**I want to** define skills once (universally)
**So that** they work the same way in all AI tools

**Acceptance Criteria:**
- [x] Skills have universal definition (`.ai-universal/skills/`)
- [x] Each tool has skill implementation (`.claude/skills/`, `.cursor/rules/`, etc.)
- [x] Skill behavior identical across tools
- [x] Documentation explains how to add skills

**Example:**
```markdown
# Universal skill definition
.ai-universal/skills/tdd-enforcement/SKILL.md
→ Defines: Trigger, behavior, enforcement

# Tool implementations
.claude/skills/test-driven-development/SKILL.md
.cursor/rules/tdd-enforcement.rule
.github/copilot-skills/tdd-enforcement.md
.openai/skills/tdd-enforcement.md
→ Each implements universal definition for their tool
```

---

#### Story 10: No Regression for Claude Code

**As a** Claude Code user
**I want** all existing features to work exactly as before
**So that** I don't lose any functionality

**Acceptance Criteria:**
- [x] All Claude commands work (`/piv_loop:*`, `/validation:*`, etc.)
- [x] All Claude skills activate automatically
- [x] All Claude agents work
- [x] All artifacts created in same format
- [x] All validation checks run
- [x] No breaking changes
- [x] Performance unchanged

**Validation:**
- [x] Test all existing features in claude-piv-skeleton
- [x] Verify feature parity in universal-ai-framework
- [x] Benchmark performance
- [x] Beta testing with existing Claude Code users

---

## 6. Core Architecture & Patterns

### High-Level Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                  UNIVERSAL AI FRAMEWORK                         │
│                  (Universal Core - Tool Agnostic)               │
└─────────────────────────────────────────────────────────────────┘
                               │
         ┌─────────────────────┼─────────────────────┐
         │                     │                     │
         ▼                     ▼                     ▼
┌────────────────┐   ┌────────────────┐   ┌────────────────┐
│  Claude Code   │   │    Cursor      │   │ GitHub Copilot │
│  (Enhanced)    │   │   (Standard)   │   │   (Standard)   │
│                │   │                │   │                │
│ - Native Cmds  │   │ - Rules Engine │   │ - Instructions │
│ - Auto Skills  │   │ - Auto Rules   │   │ - Workspace    │
│ - Agents       │   │ - Snippets     │   │ - Extensions   │
└────────────────┘   └────────────────┘   └────────────────┘
         │                     │                     │
         └─────────────────────┼─────────────────────┘
                               ▼
                    ┌────────────────┐
                    │  OpenAI Codex  │
                    │   (Standard)   │
                    │                │
                    │ - Instructions │
                    │ - Custom Sys   │
                    └────────────────┘
```

### Three-Layer Architecture

#### Layer 1: Universal Core

**Purpose:** Tool-agnostic framework that works with any AI assistant

**Directory:** `.ai-universal/`

**Contents:**
```
.ai-universal/
├── SYSTEM-PROMPT.md              # Universal system prompt
├── skills/                       # Universal skill definitions
│   ├── tdd-enforcement/
│   │   ├── SKILL.md             # Universal definition
│   │   ├── triggers.md          # When it activates
│   │   └── validation.md        # What it checks
│   ├── auto-validation/
│   ├── artifact-creation/
│   ├── conventional-commit/
│   └── code-review/
├── rules/                        # Universal rules
│   ├── 00-general.md
│   ├── 10-git.md
│   ├── 20-testing.md
│   ├── 21-testing.md
│   ├── 22-tdd-strict.md
│   ├── 30-documentation.md
│   └── 40-security.md
├── methodology/                  # PIV methodology docs
│   ├── PRIME.md
│   ├── PLAN.md
│   ├── IMPLEMENT.md
│   └── VALIDATE.md
├── prompts/                      # Universal prompt library
│   ├── prime-system.md
│   ├── plan-feature.md
│   └── execute-plan.md
└── artifacts/                    # Universal artifact structure
    ├── context/
    ├── plans/
    ├── reports/
    └── reviews/
```

**Key Principle:** Everything in `.ai-universal/` is tool-agnostic and can work with any AI assistant.

---

#### Layer 2: Universal Command System

**Purpose:** Standardized commands that work identically across all tools

**Directory:** `.ai-commands/`

**Structure:**
```
.ai-commands/
├── COMMANDS.md                   # Command reference
├── lib/
│   └── universal-prompts.md      # All command prompts
│       ├── PRIME
│       ├── PLAN
│       ├── EXECUTE
│       ├── VALIDATE
│       ├── VALIDATE:FULL
│       ├── REVIEW
│       ├── REVIEW:FIX
│       ├── REPORT:EXECUTION
│       ├── REPORT:SYSTEM
│       └── COMMIT
├── implementations/              # Tool-specific command invocation
│   ├── claude/
│   │   └── commands/            # Native command definitions
│   ├── cursor/
│   │   ├── .cursorrules         # Command routing
│   │   └── snippets/            # Text expansion
│   ├── copilot/
│   │   └── copilot-instructions.md
│   ├── codex/
│   │   └── codex-instructions.md
│   └── manual/
│       └── prompts/             # Copy-paste prompts
└── setup/
    └── install.sh
```

**Key Principle:** Commands are defined once (universally) and implemented per-tool.

---

#### Layer 3: Tool-Specific Implementations

**Purpose:** Optimize universal framework for each AI tool's native capabilities

**Structure:**
```
.claude/                          # Claude-specific (enhanced)
├── CLAUDE.md
├── PIV-METHODOLOGY.md
├── commands/                     # Native commands
│   ├── piv_loop/
│   ├── validation/
│   ├── bug_fix/
│   └── product/
├── skills/                       # Auto-activating skills
│   ├── test-driven-development/
│   ├── test-writing/
│   ├── api-design/
│   ├── security/
│   ├── code-review/
│   ├── validation:validate/
│   ├── validation:code-review/
│   └── validation:execution-report/
└── agents/                       # Agent artifacts

.cursor/                          # Cursor-specific (standard)
├── .cursorrules                  # Universal command routing
├── skills/                       # Cursor rule implementations
│   ├── tdd-enforcement.rule
│   ├── auto-validation.rule
│   └── artifact-creation.rule
└── snippets/                     # Text expansion shortcuts

.github/                          # Copilot-specific (standard)
├── copilot-instructions.md       # Universal prompts
└── copilot-skills/               # Copilot skill implementations

.openai/                          # Codex-specific (standard)
├── codex-instructions.md         # Universal prompts
└── skills/                       # Codex skill implementations
```

**Key Principle:** Each tool has optimized implementation of universal features.

---

### Key Design Patterns

#### 1. Progressive Enhancement

**Base:** Universal prompts (all tools)
```
User: /prime
→ Loads universal prompt from .ai-commands/lib/universal-prompts.md
→ Works with ANY AI tool
```

**Better:** Tool-specific commands
```
Claude: /prime (native command)
Cursor: @workspace /prime (via .cursorrules)
Copilot: /prime (via instructions)
```

**Best:** Automatic features
```
Claude: Auto-skill activates
Cursor: Auto-rule activates
Copilot: Auto-instruction applies
```

---

#### 2. Command Pattern

**Universal Structure:**
```
Command Name: /prime
Universal Prompt: .ai-commands/lib/universal-prompts.md#PRIME
Tool Implementations:
  - Claude: Native /piv_loop:prime command
  - Cursor: .cursorrules routing
  - Copilot: Instructions file
  - Codex: Instructions file
Result: Same behavior, different invocation
```

---

#### 3. Skill Pattern

**Universal Definition:**
```yaml
name: tdd-enforcement
trigger: writing implementation code
behavior: enforce RED-GREEN-REFACTOR
enforcement: strict (delete code if violated)
```

**Tool Implementations:**
```
Claude: Auto-activating skill (native)
Cursor: Rule in .cursorrules
Copilot: Instruction in copilot-instructions.md
Codex: Instruction in codex-instructions.md
```

**Result:** Same skill behavior, different tool mechanisms.

---

#### 4. Artifact Pattern

**Universal Structure:**
```
.ai-universal/artifacts/{type}/{name}-{timestamp}.md

Types:
- context/   → Context artifacts (prime phase)
- plans/     → Plan artifacts (plan phase)
- reports/   → Validation/execution/system reports
- reviews/   → Code reviews, RCAs
```

**All tools create artifacts in same structure.**

---

#### 5. PIV Methodology Pattern

**Phase-Based Workflow:**
```
1. PRIME (Context Agent)
   - Load codebase understanding
   - Create context artifact
   - Commit: "prime: load context for [feature]"

2. PLAN (Planning Agent)
   - Create implementation plan
   - Create plan artifact
   - Get user approval
   - Commit: "plan: [feature description]"

3. IMPLEMENT (Implementation Agent)
   - Execute plan with TDD (RED-GREEN-REFACTOR)
   - Auto-validation activates
   - Create execution report
   - Commit: "feat: [feature]"

4. VALIDATE (Validation Agent)
   - Runs automatically after implement
   - Create validation report
   - If fixes needed: Commit: "chore: fix validation issues"

5. SYSTEM REVIEW (Optional)
   - Analyze implementation vs plan
   - Create system review artifact
   - Commit: "docs: add system review for [feature]"
```

**Result:** Consistent workflow, consistent commits, clear history.

---

### Technology Integration Pattern

**How Technologies Are Supported:**

```
technologies/
├── backend/spring-boot/
│   ├── README.md
│   ├── rules/                   # Spring-specific rules
│   │   ├── api-design.md
│   │   └── database.md
│   ├── reference/               # Best practices
│   └── examples/                # Code examples
└── frontend/react/
    ├── README.md
    ├── rules/                   # React-specific rules
    ├── reference/               # Best practices
    └── examples/                # Code examples
```

**Each technology template includes:**
- Technology-specific rules (auto-load when working with that tech)
- Best practices reference
- Code examples
- Integration guides

---

## 7. Tools/Features

### Universal Command System

**Complete Command Catalog:**

| Command | Purpose | Claude | Cursor | Copilot | Codex | Universal |
|---------|---------|--------|--------|---------|-------|-----------|
| `/prime` | Load context | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/plan` | Create plan | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/execute` | Implement (TDD) | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/validate` | Quick validation | ✅ Auto | ✅ Rule | ✅ Auto | ✅ Auto | ✅ |
| `/validate:full` | Comprehensive | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/review` | Code review | ✅ Auto | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/review:fix` | Fix issues | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/report:exec` | Execution report | ✅ Auto | ✅ Rule | ✅ Auto | ✅ Auto | ✅ |
| `/report:sys` | System review | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/commit` | Conventional commit | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/rca` | Root cause analysis | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/fix` | Bug fix | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |
| `/prd` | Requirements doc | ✅ Native | ✅ Rule | ✅ Instr | ✅ Instr | ✅ |

**Command Aliases:**
- `/p` → `/prime`
- `/pl` → `/plan`
- `/x` → `/execute`
- `/v` → `/validate`
- `/vv` → `/validate:full`
- `/r` → `/review`
- `/c` → `/commit`

---

### Validation System

**Complete Validation Pipeline:**

**1. Quick Validation (`/validate`)**
- Run tests
- Check coverage
- TDD compliance
- Duration: Seconds

**2. Full Validation (`/validate:full`)**
- Environment safety check
- Build verification
- All tests (unit, integration, e2e)
- Code quality analysis
- Coverage analysis (≥80% target)
- Security scanning
- Dependency auditing
- TDD compliance check
- Pragmatic Programmer check
- Rule compliance
- Duration: Minutes

**3. Code Review (`/review`)**
- Code quality checks
- Bug detection
- Rule compliance
- TDD verification
- Security issues
- Performance concerns

**4. Review Fix (`/review:fix`)**
- Automatic issue fixing
- TDD-compliant fixes
- Re-validation
- Confirmation before commit

---

### Skill System

**Universal Skills + Tool Implementations:**

| Skill | Purpose | Claude | Cursor | Copilot | Codex |
|-------|---------|--------|--------|---------|-------|
| **TDD Enforcement** | Enforce RED-GREEN-REFACTOR | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Test Writing** | Given-When-Then structure | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Auto Validation** | Validate after execute | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Artifact Creation** | Create artifacts | ✅ Auto-agent | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Conventional Commit** | Standardize commits | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Code Review** | Quality checks | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **API Design** | REST best practices | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |
| **Security** | Security guidelines | ✅ Auto-skill | ✅ Auto-rule | ✅ Auto-instr | ✅ Auto-instr |

---

### Artifact System

**Complete Artifact Catalog:**

| Artifact Type | Location | Created By | Purpose |
|---------------|----------|------------|---------|
| **Context** | `.ai-universal/artifacts/context/` | `/prime` | Codebase understanding |
| **Plan** | `.ai-universal/artifacts/plans/` | `/plan` | Implementation roadmap |
| **Validation Report** | `.ai-universal/artifacts/reports/` | `/validate:full` | Quality verification |
| **Execution Report** | `.ai-universal/artifacts/reports/` | `/report:execution` | Implementation summary |
| **System Review** | `.ai-universal/artifacts/reports/` | `/report:system` | Process analysis |
| **Code Review** | `.ai-universal/artifacts/reviews/` | `/review` | Quality assessment |
| **RCA** | `.ai-universal/artifacts/reviews/` | `/rca` | Bug analysis |

---

### Agent System

**Universal Agent Definitions:**

| Agent | Phase | Purpose | Artifacts Created |
|-------|-------|---------|-------------------|
| **Context Agent** | Prime | Load codebase understanding | Context artifacts |
| **Planning Agent** | Plan | Create detailed plans | Plan artifacts |
| **Implementation Agent** | Implement | Execute with TDD | Execution reports |
| **Validation Agent** | Validate | Verify quality | Validation reports |
| **Review Agent** | Any | Code quality | Review artifacts |

---

### Git Workflow Features

**Complete Git Integration:**

- **Conventional Commits** - Auto-generate from changes
- **Main Branch Protection** - No direct commits to main
- **Feature Branch Workflow** - All changes via PR
- **Phase-Based Commits** - One commit per PIV phase
- **Atomic Commits** - Small, focused changes
- **Commit Message Generator** - Analyze changes, generate message
- **Commit Hooks** - Enforce standards (future)

---

### Technology Templates

**Supported Technologies:**

| Category | Technology | Status | Features |
|----------|------------|--------|----------|
| **Backend** | Spring Boot | ✅ Stable | API design rules, database patterns, examples |
| **Backend** | Node.js + Express | ✅ Stable | Middleware patterns, async best practices |
| **Backend** | Python + FastAPI | ✅ Stable | Async patterns, type hints, testing |
| **Frontend** | React + TypeScript | ✅ Stable | Component patterns, hooks, state management |
| **Database** | PostgreSQL | ✅ Stable | Schema design, query patterns, indexing |
| **DevOps** | Docker | ✅ Stable | Containerization, dockerfiles, compose |

---

## 8. Technology Stack

### Universal Core

**Language:** None (documentation and prompts)

**Configuration Files:**
- Markdown (`.md`) - Documentation, prompts, artifacts
- YAML (`.yml`) - GitHub Actions, configuration
- JSON (`.json`) - VS Code snippets, tool configs
- Shell scripts (`.sh`) - Installation, commands

**Dependencies:** None (standalone framework)

---

### Tool-Specific Stacks

#### Claude Code
- **Skills System:** Native (built into Claude Code)
- **Command System:** Native (`/command` syntax)
- **Agent System:** Native (multi-agent orchestration)
- **No additional dependencies**

#### Cursor
- **Rules Engine:** `.cursorrules` file
- **Snippets:** Text expansion (system-level or VS Code)
- **No additional dependencies**

#### GitHub Copilot
- **Instructions:** `.github/copilot-instructions.md`
- **Workspace:** GitHub Actions integration
- **No additional dependencies**

#### OpenAI Codex
- **Instructions:** `.openai/codex-instructions.md`
- **Custom Skills:** `.openai/skills/` directory
- **No additional dependencies**

---

### Optional Dependencies

**For Installation:**
- `curl` - Downloading installation scripts
- `git` - Version control
- `bash` - Running shell scripts

**For Development:**
- None required

**For Documentation:**
- Markdown editor (any)
- Jekyll (for GitHub Pages landing page)

---

### GitHub Pages (Landing Page)

**Tech Stack:**
- **GitHub Pages** - Free hosting
- **Jekyll** - Static site generator (built into GitHub Pages)
- **Markdown** - Content
- **Custom CSS** - Styling
- **FontAwesome** - Icons
- **Optional:** JavaScript for interactivity

---

## 9. Installation & Setup

**Universal AI Framework - Adaptive installation that detects your tech stack AND your AI tools**

---

### Installation Philosophy

The Universal AI Framework installer is **adaptive** - it detects:
1. **Your technology stack** (Spring Boot, Node, React, etc.)
2. **Your AI tools** (Claude Code, Cursor, Copilot, Codex)

Then it installs **only what you need** - no bloat, no confusion.

**Key Principle:** "Works out of the box" - One command installs everything for your specific environment.

---

### Quick Install (Recommended)

**One-line installation:**

```bash
curl -s https://raw.githubusercontent.com/galando/universal-ai-framework/main/install.sh | bash
```

**What happens:**
1. Downloads the framework
2. Detects your technology stack
3. Detects which AI tools you have
4. Shows you what it found
5. Installs appropriate configurations
6. Verifies everything works
7. Shows next steps for your tools

**Takes:** 2-3 minutes

---

### What Gets Installed

#### Universal Core (Always Installed)

These components are installed for **every** project:

```
.ai-universal/              # Universal framework core
├── SYSTEM-PROMPT.md          # Universal system prompt
├── skills/                   # Universal skill definitions
│   ├── tdd-enforcement/
│   ├── auto-validation/
│   ├── artifact-creation/
│   └── conventional-commit/
├── rules/                    # Universal rules
│   ├── 00-general.md
│   ├── 10-git.md
│   ├── 20-testing.md
│   ├── 21-testing.md
│   ├── 22-tdd-strict.md
│   ├── 30-documentation.md
│   └── 40-security.md
├── methodology/              # PIV methodology docs
│   ├── PRIME.md
│   ├── PLAN.md
│   ├── IMPLEMENT.md
│   └── VALIDATE.md
├── prompts/                  # Universal prompt library
└── artifacts/                # Artifacts you create
    ├── context/
    ├── plans/
    ├── reports/
    └── reviews/
```

#### Tool-Specific (Installed Only If You Have The Tool)

**Claude Code** (if detected):
```
.claude/                    # Claude-specific configuration
├── commands/                # Native commands
│   ├── piv_loop/
│   ├── validation/
│   ├── bug_fix/
│   └── product/
├── skills/                  # Auto-activating skills
│   ├── test-driven-development/
│   ├── validation:validate/
│   └── validation:code-review/
└── agents/                  # Agent artifacts
```

**Cursor** (if detected):
```
.cursor/                    # Cursor-specific configuration
├── .cursorrules             # Universal command routing
└── skills/                  # Cursor rule implementations
    ├── tdd-enforcement.rule
    ├── auto-validation.rule
    └── artifact-creation.rule
```

**GitHub Copilot** (if detected):
```
.github/                    # Copilot-specific configuration
├── copilot-instructions.md # Universal prompts
└── copilot-skills/          # Copilot skill definitions
```

**OpenAI Codex** (if detected):
```
.openai/                    # Codex-specific configuration
├── codex-instructions.md   # Universal prompts
└── skills/                  # Codex skill implementations
```

#### Technology Templates (Based on Your Stack)

Only templates for detected technologies are installed:

```
technologies/
├── backend/spring-boot/     # If Spring Boot detected
├── backend/node-express/    # If Node.js detected
├── frontend/react/          # If React detected
└── database/postgresql/     # If PostgreSQL detected
```

---

### Detection System

#### Technology Detection

The installer automatically detects:

| Technology | Detection Method | Files Checked |
|------------|-----------------|---------------|
| **Spring Boot** | `pom.xml` or `build.gradle*` | Maven/Gradle files |
| **Node.js/Express** | `package.json` | NPM package file |
| **React** | `package.json` with react/ReactDOM | React dependencies |
| **Python/FastAPI** | `requirements.txt` or `pyproject.toml` | Python package files |
| **PostgreSQL** | `*.sql` files, `migrations/` | SQL migration files |
| **Docker** | `Dockerfile`, `docker-compose.yml` | Docker config files |

**Result:** Only relevant technology templates are installed.

---

#### AI Tool Detection

The installer automatically detects:

| AI Tool | Detection Method | Indicators |
|---------|-----------------|------------|
| **Claude Code** | `.claude/` directory or Claude CLI | `.claude/` exists, `claude` command |
| **Cursor** | `.cursorrules` or Cursor app | `.cursorrules` exists, `/Applications/Cursor.app` |
| **GitHub Copilot** | `.github/copilot-instructions.md` | Copilot instructions file |
| **OpenAI Codex** | `.openai/` directory or Codex app | `.openai/` exists, `/Applications/Codex.app` |

**Result:** Only configurations for tools you actually have are installed.

---

### Installation Modes

#### Mode 1: Fully Automatic (Default)

Let the installer detect everything:

```bash
curl -s https://raw.githubusercontent.com/galando/universal-ai-framework/main/install.sh | bash
```

**Process:**
1. Detects your technology stack
2. Detects your AI tools
3. Shows summary:
   ```
   Detected Technologies:
   ✓ Spring Boot (Java 17)
   ✓ React (TypeScript)

   Detected AI Tools:
   ✓ Claude Code
   ✓ Cursor

   Ready to install?
   [Y/n]
   ```
4. Installs configurations for detected tools
5. Verifies each tool integration
6. Shows tool-specific next steps

**Use when:** You want the fastest, easiest installation.

---

#### Mode 2: Interactive Selection

Choose what gets installed:

```bash
# Download and run interactively
git clone https://github.com/galando/universal-ai-framework.git /tmp/uai
cd /tmp/uai
./install.sh --interactive
```

**Process:**
1. Shows detection results
2. Asks which technologies to install:
   ```
   Select technologies to install:
   [✓] Spring Boot
   [✓] React
   [ ] Node.js (not detected)
   [ ] Python (not detected)
   ```
3. Asks which AI tools to configure:
   ```
   Select AI tools to configure:
   [✓] Claude Code
   [✓] Cursor
   [ ] GitHub Copilot (not detected)
   [ ] OpenAI Codex (not detected)
   ```
4. Installs only selected items

**Use when:** You want control over what gets installed.

---

#### Mode 3: Targeted Installation

Install for specific AI tool only:

```bash
# Install for Claude Code only
./install.sh --tool claude

# Install for Cursor only
./install.sh --tool cursor

# Install for GitHub Copilot only
./install.sh --tool copilot

# Install for OpenAI Codex only
./install.sh --tool codex

# Install for multiple tools
./install.sh --tool claude,cursor
```

**Use when:** You want to add support for a specific tool later.

---

### Tool-Specific Setup Guides

After installation, each AI tool requires specific setup steps.

#### Claude Code Setup

**If detected and installed:**

```bash
╔═══════════════════════════════════════════════════════════╗
║              Claude Code Integration Installed              ║
╚═══════════════════════════════════════════════════════════╝

✓ .claude/commands/ installed
✓ .claude/skills/ installed
✓ .claude/agents/ configured
✓ All native commands verified

Next Steps:
1. Restart Claude Code
2. Try: /piv_loop:prime
3. Read: docs/getting-started/claude-code.md
```

**Manual setup if not detected:**
```bash
1. Install Claude Code: https://claude.ai/code
2. Run: curl -s https://.../install.sh | bash -s -- --tool claude
3. Restart Claude Code
4. Verify: /piv_loop:prime
```

**Verification:**
```bash
# In Claude Code, run:
/piv_loop:prime

# Should output:
✓ Context loaded: [your project type]
✓ Artifact: .ai-universal/artifacts/context/prime-{timestamp}.md
```

---

#### Cursor Setup

**If detected and installed:**

```bash
╔═══════════════════════════════════════════════════════════╗
║                  Cursor Integration Installed               ║
╚═══════════════════════════════════════════════════════════╝

✓ .cursor/.cursorrules installed
✓ Cursor skills configured
✓ Text expansion snippets created

Next Steps:
1. Restart Cursor
2. Try: Type /prime in chat
3. Read: docs/getting-started/cursor.md
```

**Manual setup if not detected:**
```bash
1. Install Cursor: https://cursor.sh
2. Run: curl -s https://.../install.sh | bash -s -- --tool cursor
3. Restart Cursor
4. Verify: Type /prime in chat
```

**Verification:**
```bash
# In Cursor chat, type:
/prime

# Should output:
✓ Context loaded: [your project type]
✓ Artifact: .ai-universal/artifacts/context/prime-{timestamp}.md
```

---

#### GitHub Copilot Setup

**If detected and installed:**

```bash
╔═══════════════════════════════════════════════════════════╗
║              GitHub Copilot Integration Installed            ║
╚═══════════════════════════════════════════════════════════╝

✓ .github/copilot-instructions.md installed
✓ Copilot Workspace integration configured
✓ Copilot skills defined

Next Steps:
1. Restart your editor (VS Code, JetBrains, etc.)
2. Open Copilot Workspace
3. Try: /prime
4. Read: docs/getting-started/copilot.md
```

**Manual setup if not detected:**
```bash
1. Install GitHub Copilot: https://github.com/features/copilot
2. Run: curl -s https://.../install.sh | bash -s -- --tool copilot
3. Restart editor
4. Open Copilot Workspace
5. Verify: /prime
```

**Verification:**
```bash
# In Copilot Workspace, type:
/prime

# Should output:
✓ Context loaded: [your project type]
✓ Artifact: .ai-universal/artifacts/context/prime-{timestamp}.md
```

---

#### OpenAI Codex Setup

**If detected and installed:**

```bash
╔═══════════════════════════════════════════════════════════╗
║               OpenAI Codex Integration Installed              ║
╚═══════════════════════════════════════════════════════════╝

✓ .openai/codex-instructions.md installed
✓ Codex skills configured
✓ Universal prompts integrated

Next Steps:
1. Restart Codex app
2. Try: /prime
3. Read: docs/getting-started/codex.md
```

**Manual setup if not detected:**
```bash
1. Access OpenAI Codex: https://openai.com/codex
2. Run: curl -s https://.../install.sh | bash -s -- --tool codex
3. Restart Codex
4. Verify: /prime
```

**Verification:**
```bash
# In Codex, type:
/prime

# Should output:
✓ Context loaded: [your project type]
✓ Artifact: .ai-universal/artifacts/context/prime-{timestamp}.md
```

---

### Verification System

#### Automatic Verification

The installer automatically verifies all components:

```bash
═══════════════════════════════════════════════════════════════════
                      Verification Report
═══════════════════════════════════════════════════════════════════

Universal Core:
✓ .ai-universal/ directory exists
✓ Universal rules loaded (7 rules)
✓ PIV methodology docs present
✓ Universal skill definitions present

Technology Integration:
✓ Spring Boot rules detected
✓ React rules detected
✓ Technology templates present

AI Tool Integration:
✓ Claude Code: Commands verified
✓ Cursor: .cursorrules verified
✓ GitHub Copilot: Instructions verified
✓ OpenAI Codex: Instructions verified

Overall: ✓ ALL CHECKS PASSED (12/12)

Installation successful!
```

#### Manual Verification

Verify each tool individually:

**Claude Code:**
```bash
# In Claude Code
/piv_loop:prime

# Expected output:
✓ Context loaded
✓ Project type: Spring Boot
✓ Tech stack: Java 17, Spring Boot 3.x
✓ Artifact created
```

**Cursor:**
```bash
# In Cursor chat
/prime

# Expected output:
✓ Context loaded
✓ Project type: Spring Boot
✓ Tech stack: Java 17, Spring Boot 3.x
✓ Artifact created
```

**GitHub Copilot:**
```bash
# In Copilot Workspace
/prime

# Expected output:
✓ Context loaded
✓ Project type: Spring Boot
✓ Tech stack: Java 17, Spring Boot 3.x
✓ Artifact created
```

**OpenAI Codex:**
```bash
# In Codex
/prime

# Expected output:
✓ Context loaded
✓ Project type: Spring Boot
✓ Tech stack: Java 17, Spring Boot 3.x
✓ Artifact created
```

---

### Installation Script Design

The installer script (`install.sh`) includes:

#### Detection Functions

```bash
# Technology Detection
detect_spring_boot() {
    if [ -f "pom.xml" ] || [ -f "build.gradle" ] || [ -f "build.gradle.kts" ]; then
        return 0
    fi
    return 1
}

detect_node() {
    if [ -f "package.json" ]; then
        return 0
    fi
    return 1
}

detect_react() {
    if [ -f "package.json" ] && grep -q "react" package.json; then
        return 0
    fi
    return 1
}

# AI Tool Detection
detect_claude_code() {
    if [ -d ".claude" ] || command -v claude &> /dev/null; then
        return 0
    fi
    return 1
}

detect_cursor() {
    if [ -f ".cursorrules" ] || [ -d "/Applications/Cursor.app" ]; then
        return 0
    fi
    return 1
}

detect_copilot() {
    if [ -f ".github/copilot-instructions.md" ]; then
        return 0
    fi
    return 1
}

detect_codex() {
    if [ -d ".openai" ] || [ -d "/Applications/Codex.app" ]; then
        return 0
    fi
    return 1
}
```

#### Installation Functions

```bash
install_claude() {
    print_info "Installing Claude Code integration..."

    # Copy .claude/ directory
    cp -r "$SOURCE_DIR/.claude/" .claude/

    # Verify commands
    if [ -d ".claude/commands" ]; then
        print_success "✓ Claude commands installed"
    else
        return 1
    fi

    # Verify skills
    if [ -d ".claude/skills" ]; then
        print_success "✓ Claude skills installed"
    else
        return 1
    fi

    return 0
}

install_cursor() {
    print_info "Installing Cursor integration..."

    mkdir -p .cursor
    cp "$SOURCE_DIR/.cursor/.cursorrules" .cursor/
    cp -r "$SOURCE_DIR/.cursor/skills/" .cursor/

    if [ -f ".cursor/.cursorrules" ]; then
        print_success "✓ Cursor configuration installed"
        return 0
    fi

    return 1
}

install_copilot() {
    print_info "Installing GitHub Copilot integration..."

    mkdir -p .github
    cp "$SOURCE_DIR/.github/copilot-instructions.md" .github/

    if [ -f ".github/copilot-instructions.md" ]; then
        print_success "✓ Copilot instructions installed"
        return 0
    fi

    return 1
}

install_codex() {
    print_info "Installing OpenAI Codex integration..."

    mkdir -p .openai
    cp "$SOURCE_DIR/.openai/codex-instructions.md" .openai/
    cp -r "$SOURCE_DIR/.openai/skills/" .openai/

    if [ -f ".openai/codex-instructions.md" ]; then
        print_success "✓ Codex configuration installed"
        return 0
    fi

    return 1
}
```

---

### Troubleshooting Installation

#### Problem: AI Tool Not Detected

**Symptom:** Installer didn't detect your AI tool

**Solutions:**

```bash
# Manually specify the tool
./install.sh --tool claude
./install.sh --tool cursor
./install.sh --tool copilot
./install.sh --tool codex

# Or use interactive mode
./install.sh --interactive
```

---

#### Problem: Commands Not Recognized

**Symptom:** `/prime` or other commands don't work in AI tool

**Solutions:**

1. **Restart the AI tool** - Most configuration requires restart
2. **Check tool-specific file exists:**
   - Claude: `.claude/commands/piv_loop/prime.md`
   - Cursor: `.cursor/.cursorrules`
   - Copilot: `.github/copilot-instructions.md`
   - Codex: `.openai/codex-instructions.md`
3. **Reinstall for that tool:**
   ```bash
   ./install.sh --tool [tool-name]
   ```

---

#### Problem: Technology Not Detected

**Symptom:** Your technology stack wasn't detected

**Solutions:**

```bash
# Manually install technology template
cp -r technologies/backend/spring-boot/ .
cp -r technologies/frontend/react/ .

# Or use interactive mode
./install.sh --interactive
```

---

#### Problem: Partial Installation

**Symptom:** Only some tools were configured

**Solutions:**

```bash
# Re-run installer for missing tools
./install.sh --tool [missing-tool]

# Example: Add Cursor to existing Claude installation
./install.sh --tool cursor
```

---

#### Problem: Backup Restoration Needed

**Symptom:** Installation broke something, need to undo

**Solutions:**

```bash
# Run uninstall script
./uninstall.sh

# This will:
# 1. Show backup location
# 2. Ask if you want to restore
# 3. Remove all framework files
# 4. Restore your backup
```

---

### Uninstallation

#### Uninstall Everything

```bash
./uninstall.sh
```

**Process:**
1. Shows what will be removed
2. Offers to restore backup first
3. Removes all framework files:
   - `.ai-universal/`
   - `.ai-commands/`
   - `.claude/` (if installed by framework)
   - `.cursor/` (if installed by framework)
   - `.github/copilot-instructions.md` (if installed by framework)
   - `.openai/` (if installed by framework)
4. Cleans up backup metadata

---

#### Uninstall Specific Tool

```bash
# Uninstall just Claude Code integration
./uninstall.sh --tool claude

# Uninstall just Cursor integration
./uninstall.sh --tool cursor

# Uninstall just Copilot integration
./uninstall.sh --tool copilot

# Uninstall just Codex integration
./uninstall.sh --tool codex
```

**Preserves:** Other tool integrations and universal core

---

#### Keep Universal Core, Remove Tools

```bash
# Remove all tool integrations, keep universal framework
./uninstall.sh --tools-only

# This keeps:
# - .ai-universal/ (universal core)
# - technologies/ (templates)
# But removes:
# - .claude/
# - .cursor/
# - .github/copilot-instructions.md
# - .openai/
```

---

### Installation Success Criteria

Installation is considered successful when:

**Universal Core:**
- [x] `.ai-universal/` directory exists
- [x] All universal rules present
- [x] PIV methodology docs present
- [x] Universal skill definitions present

**AI Tool Integration (for each detected tool):**
- [x] Tool-specific directory/file created
- [x] Commands verified (Claude)
- [x] Rules configured (Cursor)
- [x] Instructions installed (Copilot, Codex)
- [x] Tool-specific verification passes

**Technology Integration:**
- [x] Detected technologies have templates
- [x] Technology-specific rules present
- [x] Technology documentation accessible

**Overall:**
- [x] All verification checks pass
- [x] User can run `/prime` in their AI tool(s)
- [x] Artifacts created successfully
- [x] Next steps shown clearly

---

### Installation Documentation

**Complete documentation set:**

1. **Main Installation Guide** (`docs/getting-started/01-installation.md`)
   - Overview and quick install
   - Detection explanation
   - Installation modes
   - Tool-specific setup
   - Verification
   - Troubleshooting
   - Uninstallation

2. **Tool-Specific Guides** (`docs/getting-started/tool-guides/`)
   - `claude-code.md` - Claude Code setup and usage
   - `cursor.md` - Cursor setup and usage
   - `copilot.md` - GitHub Copilot setup and usage
   - `codex.md` - OpenAI Codex setup and usage

3. **Installation Script Documentation** (`scripts/README.md`)
   - Script architecture
   - Detection algorithms
   - Installation functions
   - Verification system
   - Extending the installer

---

## 10. Security & Configuration

### Security Scope

**✅ In Scope (Security Features):**

**Framework Security:**
- [x] Security rules and guidelines (`.ai-universal/rules/40-security.md`)
- [x] Security scanning in validation (`/validate:full`)
- [x] Dependency vulnerability checks
- [x] Sensitive data detection (passwords, API keys)
- [x] SQL injection prevention checks
- [x] XSS prevention checks
- [x] Security best practices enforcement

**User Security:**
- [x] No sensitive data in artifacts
- [x] No API keys or secrets stored in framework
- [x] Local execution only (no network calls)
- [x] No data transmission to external services

**❌ Out of Scope:**
- Authentication (no user accounts)
- Authorization (no permissions)
- Encryption (no data transmission)
- Audit logging (local only)
- Access control (local files only)

---

### Configuration Management

**Environment Variables:** None required for framework

**Configuration Files:**

**Universal:**
- `.ai-universal/SYSTEM-PROMPT.md` - Universal system prompt
- `.ai-commands/lib/universal-prompts.md` - Command prompts

**Tool-Specific:**
- `.claude/CLAUDE.md` - Claude configuration
- `.cursor/.cursorrules` - Cursor configuration
- `.github/copilot-instructions.md` - Copilot configuration
- `.openai/codex-instructions.md` - Codex configuration

**Technology-Specific:**
- `technologies/*/rules/` - Technology-specific rules
- `technologies/*/reference/` - Best practices

**User Configuration:**
- None required for MVP
- Future: `.ai-framework-config.json` for customization

---

### Deployment Considerations

**Local Development:**
- No deployment required
- Works entirely locally
- No network dependencies

**Distribution:**
- GitHub repository
- Installation via curl/bash script
- Manual download and setup

**Documentation:**
- GitHub Pages (free hosting)
- Static site (Jekyll)
- Custom domain optional

**Updates:**
- Git pull for updates
- No automatic updates (MVP)
- Future: Update notification system

---

## 11. API Specification

**Not Applicable** - This is not a networked service or API.

However, we define "Command APIs" for consistency:

### Command API: `/prime`

**Invocation:**
- Claude: `/piv_loop:prime` (native)
- Cursor: `@workspace /prime` (via .cursorrules)
- Copilot: `/prime` (via instructions)
- Codex: `/prime` (via instructions)

**Input:** None (or optional topic for targeted prime)

**Output:**
```
✓ Context loaded
✓ Project type: [detected type]
✓ Tech stack: [list]
✓ Key patterns: [list]
✓ Artifact: .ai-universal/artifacts/context/prime-{timestamp}.md
```

### Command API: `/execute`

**Invocation:**
- Claude: `/piv_loop:execute [plan-name]`
- Cursor: `/execute [plan-name]`
- Copilot: `/execute [plan-name]`
- Codex: `/execute [plan-name]`

**Input:**
- Plan name (optional, defaults to latest)

**Output:**
```
Executing plan: [plan-name]
Step 1/8: [step description]
✓ Test written (RED) - FAILING ✓
✓ Implementation (GREEN) - PASSING ✓
✓ Refactored (REFACTOR) - PASSING ✓
...
✓ All steps complete
✓ Auto-validating...
✓ Tests: 47/47 passing
✓ Coverage: 89%
✓ Ready to commit
```

### Command API: `/validate:full`

**Invocation:**
- Claude: `/validation:validate`
- Cursor: `/validate:full`
- Copilot: `/validate:full`
- Codex: `/validate:full`

**Input:** None (or target feature/directory)

**Output:**
```
════════════════════════════════════════
 VALIDATION REPORT
════════════════════════════════════════

✓ Environment: Safe (DEV mode)
✓ Build: Success (2.4s)
✓ Tests: 47/47 passing (100%)
✓ Coverage: 89% (target: 80%)
✓ Code Quality: Good
✓ Security: No vulnerabilities
✓ Dependencies: All up to date
✓ TDD Compliance: Tests before code
✓ Pragmatic Programmer: Applied

Overall: ✓ PASSED

Report: .ai-universal/artifacts/reports/validation-full-{timestamp}.md
```

---

## 12. Success Criteria

### MVP Success Definition

**The MVP is successful when:**

1. A developer can use `/prime`, `/plan`, `/execute`, `/validate` with **Claude, Cursor, Copilot, or Codex** and get equivalent results
2. Claude Code users retain all existing functionality (no regression)
3. Cursor, Copilot, and Codex users have **feature parity** with Claude Code
4. New users can install and start using the framework in **< 10 minutes**
5. Documentation clearly explains how to use with each supported tool
6. The framework is truly tool-agnostic (no hardcoded assumptions about AI tools)
7. All artifacts are created in consistent structure regardless of tool
8. All validation checks run identically across all tools

---

### Functional Requirements

**Core Workflow (All Tools):**
- [x] `/prime` loads context in all 4 tools
- [x] `/plan` creates implementation plans in all 4 tools
- [x] `/execute` follows TDD cycle in all 4 tools
- [x] `/validate:full` runs comprehensive validation in all 4 tools
- [x] `/review` performs code review in all 4 tools
- [x] `/commit` creates atomic commits in all 4 tools
- [x] `/rca` performs root cause analysis in all 4 tools
- [x] `/fix` implements bug fixes in all 4 tools

**Automatic Features (All Tools):**
- [x] TDD enforcement activates automatically in all 4 tools
- [x] Validation runs automatically after execute in all 4 tools
- [x] Artifacts created automatically in all 4 tools
- [x] Code review activates before commits (Claude) or available (others)

**Tool Integration:**
- [x] Claude Code: Native command support + auto-features (no regression)
- [x] Cursor: `.cursorrules` + snippets working
- [x] GitHub Copilot: Instructions file + workspace integration working
- [x] OpenAI Codex: Instructions file + custom system working

**Documentation:**
- [x] Universal command reference
- [x] Tool-specific setup guides (Claude, Cursor, Copilot, Codex)
- [x] Installation script working
- [x] Migration guide from claude-piv-skeleton
- [x] Prompt library for manual tools
- [x] GitHub Pages landing page
- [x] Feature documentation complete
- [x] Troubleshooting guide

**Quality:**
- [x] All universal rules extracted and tested
- [x] All command prompts working with generic AI
- [x] Artifact structure consistent across tools
- [x] No regression in Claude Code functionality
- [x] All validation checks working in all tools
- [x] All skills activating in all tools

---

### Quality Indicators

**Usability:**
- Time to first successful `/prime`: < 2 minutes
- Time to complete first feature: < 30 minutes
- Documentation clarity score: > 4/5 (user feedback)
- Installation success rate: > 95%

**Compatibility:**
- Works with all 4 AI tools (Claude, Cursor, Copilot, Codex)
- Works with all 6 technology templates (Spring Boot, Node, FastAPI, React, PostgreSQL, Docker)
- No tool-specific breaking changes
- Feature parity across all tools

**Reliability:**
- Commands work consistently across tools
- Artifact creation succeeds > 95% of time
- Installation succeeds > 90% of time
- Validation passes consistently for correct code

**Maintainability:**
- Code duplication < 10%
- Documentation coverage 100%
- Clear separation of universal vs. tool-specific
- Easy to add new tools (documented process)

**Performance:**
- `/prime` completes in < 30 seconds
- `/execute` (simple feature) completes in < 5 minutes
- `/validate:full` completes in < 2 minutes
- No performance regression in Claude Code

---

### User Experience Goals

**For Claude Code Users:**
- "I didn't lose any functionality"
- "Everything works the same"
- "I can still use auto-features"
- "No learning curve"

**For Cursor/Copilot/Codex Users:**
- "Setup was easy and clear"
- "Commands work as expected"
- "Documentation is helpful"
- "I can be productive immediately"
- "Feature parity with Claude"

**For Switchers:**
- "I can move between tools easily"
- "My workflow is consistent"
- "I don't have to relearn everything"
- "Artifacts are the same"

**For Teams:**
- "Consistent quality across team"
- "Easy to review AI work via artifacts"
- "Onboarding is straightforward"
- "Standards are enforced"

---

## 13. Implementation Phases

### Phase 0: Preparation (Week 0)

**Goal:** Set up for successful fork and development

**Deliverables:**
- [x] Create `universal-ai-framework` repository on GitHub
- [x] Fork from `claude-piv-skeleton`
- [x] Set up local development environment
- [x] Create development branch (`feature/universal-framework`)
- [x] Set up project board (GitHub Projects)
- [x] Review all existing features in claude-piv-skeleton

**Validation Criteria:**
- New repository exists
- Fork is complete
- Local environment works
- All features documented

**Estimated Effort:** 4 hours

---

### Phase 1: Universal Core Extraction (Week 1-2)

**Goal:** Extract universal components from Claude-specific structure

**Deliverables:**
- [x] Create `.ai-universal/` directory structure
- [x] Extract universal rules from `.claude/rules/` to `.ai-universal/rules/`
- [x] Extract PIV methodology to `.ai-universal/methodology/`
- [x] Create `.ai-commands/` directory
- [x] Create universal prompts in `.ai-commands/lib/universal-prompts.md`
- [x] Create universal skill definitions in `.ai-universal/skills/`
- [x] Create artifact directory structure in `.ai-universal/artifacts/`
- [x] Update repository name in all files

**Validation Criteria:**
- `.ai-universal/` structure exists and is complete
- Universal rules contain no Claude-specific references
- Universal prompts work with generic AI (manual testing)
- Artifact structure is tool-agnostic
- All existing features accounted for

**Estimated Effort:** 40 hours

---

### Phase 2: Claude Code Preservation (Week 2-3)

**Goal:** Ensure Claude Code users have no regression

**Deliverables:**
- [x] Keep `.claude/` directory unchanged (additive only)
- [x] Test all Claude commands (`/piv_loop:*`, `/validation:*`, etc.)
- [x] Test all Claude skills (auto-activation)
- [x] Test all Claude agents
- [x] Verify artifact creation still works
- [x] Verify validation still runs automatically
- [x] Benchmark performance (ensure no regression)
- [x] Update `.claude/CLAUDE.md` with universal context

**Validation Criteria:**
- All Claude commands work exactly as before
- All Claude skills activate automatically
- All Claude agents work
- All artifacts created in same format
- All validation checks run
- No performance regression
- Beta tester approval (existing Claude users)

**Estimated Effort:** 20 hours

---

### Phase 3: Cursor Integration (Week 3-4)

**Goal:** Implement complete Cursor integration with feature parity

**Deliverables:**
- [x] Create `.cursor/` directory structure
- [x] Create `.cursorrules` with universal command routing
- [x] Implement TDD enforcement rule
- [x] Implement auto-validation rule
- [x] Implement artifact creation rule
- [x] Create text expansion snippets
- [x] Create Cursor setup guide
- [x] Test all commands in Cursor
- [x] Test all skills (rules) in Cursor
- [x] Verify artifact creation in Cursor
- [x] Verify validation runs in Cursor

**Validation Criteria:**
- `/prime` works in Cursor
- `/execute` works in Cursor with TDD
- `/validate:full` works in Cursor
- All skills activate via rules
- Artifacts created correctly
- Feature parity with Claude achieved
- Setup guide tested by new user

**Estimated Effort:** 30 hours

---

### Phase 4: Copilot Integration (Week 4-5)

**Goal:** Implement complete GitHub Copilot integration

**Deliverables:**
- [x] Create `.github/` directory structure
- [x] Create `copilot-instructions.md` with universal prompts
- [x] Implement Copilot-specific skill definitions
- [x] Create Copilot Workspace integration
- [x] Create Copilot setup guide
- [x] Test all commands in Copilot
- [x] Test all skills in Copilot
- [x] Verify artifact creation in Copilot
- [x] Verify validation runs in Copilot

**Validation Criteria:**
- `/prime` works in Copilot
- `/execute` works in Copilot with TDD
- `/validate:full` works in Copilot
- All skills activate via instructions
- Artifacts created correctly
- Feature parity achieved (where Copilot allows)
- Setup guide tested by new user

**Estimated Effort:** 25 hours

---

### Phase 5: Codex Integration (Week 5-6)

**Goal:** Implement complete OpenAI Codex integration

**Deliverables:**
- [x] Create `.openai/` directory structure
- [x] Create `codex-instructions.md` with universal prompts
- [x] Implement Codex-specific skill definitions
- [x] Create Codex setup guide
- [x] Test all commands in Codex
- [x] Test all skills in Codex
- [x] Verify artifact creation in Codex
- [x] Verify validation runs in Codex

**Validation Criteria:**
- `/prime` works in Codex
- `/execute` works in Codex with TDD
- `/validate:full` works in Codex
- All skills activate via instructions
- Artifacts created correctly
- Feature parity achieved
- Setup guide tested by new user

**Estimated Effort:** 25 hours

---

### Phase 6: Documentation & Landing Page (Week 6-7)

**Goal:** Create comprehensive documentation and GitHub Pages site

**Deliverables:**
- [x] Update README.md for multi-tool support
- [x] Create `docs/index.md` (landing page)
- [x] Create `docs/_config.yml` (Jekyll config)
- [x] Create `docs/_layouts/` (page templates)
- [x] Create `docs/assets/css/` (custom styling)
- [x] Create tool-specific setup guides:
  - [x] Claude Code guide
  - [x] Cursor guide
  - [x] GitHub Copilot guide
  - [x] OpenAI Codex guide
- [x] Create `docs/AGENTS.md` (universal agent concept)
- [x] Create `docs/METHODOLOGY.md` (PIV methodology)
- [x] Create `docs/skills/` documentation
- [x] Create migration guide (from claude-piv-skeleton)
- [x] Create troubleshooting guide
- [x] Update FAQ
- [x] Enable GitHub Pages

**Validation Criteria:**
- GitHub Pages site builds successfully
- Site is mobile-responsive
- All tool guides tested and working
- Documentation passes review
- Site SEO-optimized
- Loading time < 2 seconds

**Estimated Effort:** 40 hours

---

### Phase 7: Installation & Testing (Week 7-8)

**Goal:** Create installation system and comprehensive testing

**Deliverables:**
- [x] Create installation script (`install.sh`)
- [x] Create setup wizard (interactive script)
- [x] Implement technology auto-detection
- [x] Implement tool auto-detection
- [x] Create pre-install backup
- [x] Create post-install verification
- [x] Test installation on clean projects:
  - [x] Spring Boot project
  - [x] Node.js project
  - [x] React project
- [x] Test all tools with all commands
- [x] Cross-tool testing (use same project with different tools)
- [x] Performance testing
- [x] Security testing

**Validation Criteria:**
- Installation script works on all test projects
- Technology detection accurate
- Tool detection accurate
- Installation success rate > 90%
- All commands work in all tools
- Cross-tool artifact consistency verified
- No security vulnerabilities
- Performance acceptable

**Estimated Effort:** 30 hours

---

### Phase 8: Polish & Launch (Week 8-9)

**Goal:** Final polish, quality checks, and launch

**Deliverables:**
- [x] Complete code review
- [x] Update CHANGELOG.md
- [x] Create release notes (v1.0.0)
- [x] Test migration path from claude-piv-skeleton
- [x] Gather beta tester feedback (all 4 tools)
- [x] Fix critical bugs
- [x] Update badges and links in README
- [x] Prepare GitHub release
- [x] Create announcement blog post
- [x] Launch announcement (social media, forums)
- [x] Monitor issues and respond

**Validation Criteria:**
- No critical bugs remaining
- Beta tester satisfaction > 4/5 (all tools)
- Migration path tested and documented
- Release approved by maintainer
- Launch successful
- Initial community engagement positive

**Estimated Effort:** 20 hours

**Total Estimated Effort:** 234 hours (~6 weeks full-time, ~3 months part-time)

---

## 14. Future Considerations

### Post-MVP Enhancements

**v1.1 - Enhanced Tool Support (3 months after MVP)**
- Pre-built integrations for Tabnine, CodeWhisperer
- Enhanced Copilot Workspace features
- Interactive setup wizard (GUI)
- Performance optimizations

**v1.2 - Team Features (6 months after MVP)**
- Shared artifact storage (cloud/local server)
- Team analytics dashboard
- Code review collaboration features
- Team configuration management

**v1.3 - Automation (9 months after MVP)**
- CI/CD integration (GitHub Actions validation)
- Pre-commit hooks for validation
- Automatic artifact generation
- Scheduled validation runs

**v2.0 - Advanced Features (12+ months after MVP)**
- Multi-agent collaboration
- Custom command builder (GUI)
- Plugin system
- Remote execution support
- Artifact versioning and history

---

### Integration Opportunities

**Potential Partnerships:**
- **Cursor:** Official integration in Cursor marketplace
- **GitHub:** Featured Copilot Workspace template
- **OpenAI:** Official Codex integration
- **JetBrains:** IDE plugin marketplace

**Community Contributions:**
- Technology templates (Rust, Go, Django, etc.)
- Tool integrations (new AI tools as they emerge)
- Rule sets (industry-specific: healthcare, finance, etc.)
- Localization (translations of documentation)

---

### Advanced Features for Later Phases

**Artificial Intelligence:**
- Learn from user patterns
- Suggest optimizations
- Predictive validation
- Intelligent test generation

**Developer Experience:**
- Web-based configuration UI
- Visual artifact explorer
- Interactive command builder
- Real-time collaboration

**Enterprise Features:**
- SSO integration
- Audit logging
- Compliance reporting
- Custom rule sets
- On-premise deployment

---

## 15. Risks & Mitigations

### Risk 1: Tool Vendor Breaking Changes

**Risk:** AI tool vendors (Anthropic, Microsoft, OpenAI, Cursor) change their APIs or capabilities, breaking integrations.

**Impact:** High - Could break core functionality

**Probability:** Medium - Tools are evolving rapidly

**Mitigation Strategy:**
- Design for loose coupling (tool-specific layer isolated)
- Use stable, documented APIs where possible
- Create abstraction layers for tool interactions
- Monitor tool release notes and changelogs
- Maintain backward compatibility where possible
- Community feedback loop for early detection

**Contingency Plan:**
- Version tool integrations (v1, v2, etc.)
- Support multiple versions simultaneously during transition
- Clear migration guide for users
- Quick revert to previous version if critical break

---

### Risk 2: Complexity and Maintenance Burden

**Risk:** Supporting 4+ tools increases complexity and maintenance effort significantly.

**Impact:** High - Could lead to burnout or project abandonment

**Probability:** High - Multi-tool support is inherently complex

**Mitigation Strategy:**
- Keep universal core simple and stable
- Modular design (tool integrations are plugins)
- Community contributions for tool integrations
- Clear separation of concerns (universal vs. tool-specific)
- Automated testing for each tool integration
- Documentation for contributors

**Contingency Plan:**
- Deprecate underused tools if maintenance burden too high
- Focus on 2-3 most popular tools if needed
- Community adoption model for less popular tools
- Regular maintenance audits to assess sustainability

---

### Risk 3: Feature Parity Not Achievable

**Risk:** Some tools (Cursor, Copilot, Codex) may not support all features that Claude Code supports, leading to inconsistent experience.

**Impact:** High - Undermines "universal" value proposition

**Probability:** Medium - Tools have different capabilities

**Mitigation Strategy:**
- Be transparent about tool limitations in documentation
- Focus on core features that all tools can support
- Create "quality tiers" (full vs. partial feature support)
- Provide workarounds where possible
- Recommend best tool for strict quality enforcement

**Contingency Plan:**
- Document feature matrix clearly
- Be honest about which tool is best for which use case
- Focus on tools with best automation capabilities
- Consider dropping tools that can't achieve feature parity

---

### Risk 4: Claude Code User Regression

**Risk:** Changes to support universal framework break existing Claude Code functionality, alienating current users.

**Impact:** High - Loss of existing user base, trust damage

**Probability:** Low - Changes are additive, not replacing

**Mitigation Strategy:**
- Keep `.claude/` directory unchanged (additive only)
- Comprehensive testing of Claude features before release
- Beta testing with existing Claude Code users
- Clear migration guide
- Backward compatibility guarantee
- Separate branch for Claude-only version (for safety)

**Contingency Plan:**
- Maintain claude-piv-skeleton as separate option
- Quick rollback plan if critical regression found
- Support both versions during transition
- Hotfix releases for critical Claude issues

---

### Risk 5: User Adoption and Confusion

**Risk:** Users find the system too complex or confusing, or don't understand the difference between claude-piv-skeleton and universal-ai-framework.

**Impact:** High - Project fails to gain traction

**Probability:** Medium - Multi-tool complexity can confuse

**Mitigation Strategy:**
- Progressive disclosure (basic vs. advanced features)
- Clear, concise documentation
- Quick start guide (< 10 minutes to first success)
- Video tutorials for visual learners
- Examples for each tool and technology
- Active support (GitHub Issues, Discord)
- Clear explanation of claude-piv-skeleton vs. universal-ai-framework

**Contingency Plan:**
- Simplify based on user feedback
- Focus on 1-2 tools if needed
- Improve onboarding flow
- Target one user persona first (e.g., Cursor users)
- A/B test different messaging

---

### Risk 6: Quality Enforcement Inconsistency

**Risk:** Quality enforcement (TDD, validation) works well in Claude but inconsistently in other tools due to tool limitations.

**Impact:** Medium - Undermines quality value proposition

**Probability:** Medium - Tools have different automation capabilities

**Mitigation Strategy:**
- Design universal prompts that work reliably
- Test prompts with multiple AI tools (not just Claude)
- Provide feedback when tools can't enforce rules
- Document limitations of each tool
- Recommend Claude Code for strictest enforcement
- Create "quality tiers" documentation

**Contingency Plan:**
- Be transparent about tool limitations
- Focus on tools that can enforce quality well
- Create "recommended for" badges based on capabilities
- Document which features work best in which tools

---

## 16. Appendix

### Related Documents

**Internal:**
- [PIV Methodology](.claude/PIV-METHODOLOGY.md) - Core methodology documentation
- [Project Instructions](.claude/CLAUDE.md) - Quick reference
- [Skills System](docs/features/skills-system.md) - Claude Code skills
- [Strict TDD](docs/features/strict-tdd.md) - TDD enforcement

**External:**
- [Context Engineering](https://github.com/coleam00/context-engineering-intro) - Original PIV methodology
- [Habit Tracker](https://github.com/coleam00/habit-tracker) - PIV demonstration
- [Claude Code Docs](https://docs.anthropic.com/claude-code) - Claude Code documentation
- [Cursor Docs](https://cursor.sh/docs) - Cursor documentation
- [GitHub Copilot Docs](https://docs.github.com/en/copilot) - Copilot documentation
- [OpenAI Codex](https://openai.com/codex) - Codex information

### Key Dependencies

**No external dependencies** - This is a standalone documentation and configuration system.

**Optional Tools:**
- [Claude Code](https://claude.ai/code) - Anthropic's AI coding assistant
- [Cursor](https://cursor.sh) - AI-powered code editor
- [GitHub Copilot](https://github.com/features/copilot) - GitHub's AI assistant
- [OpenAI Codex](https://openai.com/codex) - OpenAI's code generation system

### Repository Structure

See Section 6 for complete directory structure.

### Glossary

- **PIV:** Prime-Implement-Validate, the core methodology
- **TDD:** Test-Driven Development, RED-GREEN-REFACTOR cycle
- **Artifact:** Document created by AI agents (context, plan, report, etc.)
- **Universal:** Works with any AI tool, not tool-specific
- **Skill:** Auto-activating behavior in AI tools
- **Agent:** Autonomous AI entity that performs tasks
- **Prompt:** Text input given to AI tools to execute commands
- **Rule:** Tool-specific implementation of universal skill
- **Validation:** Comprehensive quality verification
- **RCA:** Root Cause Analysis for bugs

### Version History

**v1.0.0 (MVP - Current)**
- Universal AI Framework
- Multi-tool support (Claude, Cursor, Copilot, Codex)
- Universal command system
- Universal artifact structure
- Tool-specific integrations
- Complete feature parity
- GitHub Pages documentation

**v0.9.0 (Parent: claude-piv-skeleton)**
- Claude Code only
- PIV methodology
- Strict TDD enforcement
- Skills system
- Agent orchestration

### Change Log

**v1.0.0 (Universal AI Framework)**
- Forked from claude-piv-skeleton
- Extracted universal core (.ai-universal/)
- Created universal command system (.ai-commands/)
- Added Cursor integration
- Added GitHub Copilot integration
- Added OpenAI Codex integration
- Created GitHub Pages documentation
- Universal skill definitions
- Complete feature parity across tools

---

## Document Approval

| Role | Name | Approval | Date |
|------|------|----------|------|
| Product Owner | Galando | ⬜ Pending | |
| Technical Lead | | ⬜ Pending | |
| Documentation | | ⬜ Pending | |

---

## Next Steps

1. **Create new repository** - `universal-ai-framework` on GitHub
2. **Fork from claude-piv-skeleton** - Preserve existing functionality
3. **Begin Phase 0** - Set up development environment
4. **Create project board** - Track implementation phases
5. **Set up GitHub Pages** - Prepare documentation site

**Questions or Feedback?**
- Open an issue on GitHub
- Contact maintainer: [galando](https://github.com/galando)
- Discussion: [GitHub Discussions](https://github.com/galando/universal-ai-framework/discussions)

---

**End of PRD v1.0.0 - Universal AI Framework**
