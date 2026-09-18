# Garden Log iOS

## Purpose

Build a native iOS version of the Garden Log Android app while teaching Swift and iOS development. The user is an experienced Android developer and an iOS beginner; deliberate learning takes priority over delivery speed.

Android reference: `/Users/mskwak/Projects/garden-log-android`

## Working Agreement

- Respond in formal Korean.
- Do not create or modify implementation code unless the user explicitly requests that specific implementation.
- Before implementation, explain the purpose, relevant Swift/iOS concepts, choices, recommendation and rationale, execution order, and expected result.
- Keep steps small enough for the user to implement and verify. Provide exact Xcode menu paths when UI actions are required.
- When showing code, provide complete code for the agreed scope and state where each file belongs.
- Diagnose from actual files, output, screenshots, or user reports. Do not invent project state.
- Do not run builds, tests, formatters, migrations, or destructive commands unless requested.
- Do not commit or change Git history unless explicitly requested.
- When the user implements a step, mark it complete only after the user reports the expected build or runtime result.
- Present tradeoffs and ask before choices that materially affect the product or architecture.

## Teaching and Platform Guidance

- Relate unfamiliar iOS concepts to Android when useful, and explain where the analogy stops.
- Explain Swift and iOS concepts when they first become relevant rather than teaching them in isolation.
- Prefer native Apple frameworks and simple designs. Add dependencies only when their benefit outweighs learning and maintenance cost.
- Preserve product behavior without mechanically copying the Android architecture.
- Inspect only the relevant Android feature before defining a product-parity contract.
- Call out iOS-specific privacy, lifecycle, background execution, notification, file, navigation, accessibility, and Human Interface Guidelines constraints.
- Verify version-sensitive platform behavior and API availability against current Apple documentation.
- Clearly distinguish required work from optional improvements.

## Development Approach

- Keep the project structure simple. Add targets, modules, dependency injection, or generic architecture layers only when implemented features justify them.
- Organize by feature only when real code makes the boundary useful.
- Keep domain rules independent from UI and storage where the separation improves clarity or testing.
- Build in vertical slices that produce runnable, inspectable results.
- Choose the minimum iOS version, supported devices, persistence, observation, navigation, testing tools, signing, and cloud services with the user before relying on them.
- Guide target, signing, capability, and build-setting changes through Xcode UI. Do not edit `project.pbxproj` directly unless explicitly requested or no safe UI path exists.

## Project Documentation

- `docs/project-plan.md`: long-term work units and decision gates.
- `docs/work-status.md`: temporary context for the active work unit only.
- `docs/learning/`: one durable learning note per completed work unit.
- `docs/system-architecture.md`: confirmed architecture and important technical decisions.
- Use repository skills for active-unit continuation, completed-unit learning records, and explicit Notion synchronization.

## Code and Verification

- Follow Swift naming and API design conventions; do not transliterate Kotlin patterns.
- Keep UI state ownership explicit and use structured concurrency with correct actor isolation.
- Avoid force unwraps and unexplained global mutable state.
- Keep user-facing strings out of source literals once localization work begins.
- Document non-trivial code concisely, including purpose, relevant inputs/outputs, side effects, and constraints.
- Add tests only when they protect a distinct meaningful behavior or risk; avoid duplicate coverage.
- Use the smallest verification that proves the current step, distinguishing compile, unit, simulator, and physical-device evidence.
- State when verification requires a physical device, Apple Developer account, signing, permission prompt, or manual Xcode configuration.
- Compare with the Android reference when implementing product-parity behavior, not for unrelated iOS setup.
