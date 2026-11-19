# Zero reports

Public structured technical reports from [Zero](https://github.com/codepetca/zero), helping students **Learn to Build**.

## Reporting status

Production collection was enabled on 2026-11-19 after [PR #386](https://github.com/codepetca/zero/pull/386) passed all hosted gates and merged. Actual native editor submission and silent automatic collector acceptance reached the hosted service, Vercel-provisioned Neon database and dedicated GitHub App. Synthetic acceptance issues are labelled `activation-test` and closed.

Automatic public reporting starts off. Zero offers one explicit public-reporting choice during first-run setup. After Allow reports, eligible unexpected errors send silently and the manual Report a problem action sends directly. Declining keeps automatic reporting off; opted-out manual submissions require one-off public confirmation. VS Code telemetry settings also gate automatic reports.

The reporting-enabled collector requires a separate editor release. Existing published installers are not updated by enabling the website service. See the [current operation and acceptance record](https://github.com/codepetca/zero/blob/main/docs/PROBLEM-REPORTING.md) for deployment and reconciliation status.

## What a report contains

The service accepts a fixed schema containing software versions, operating system and architecture, the failed operation and stage, a stable error code, timestamps, a random report ID and bounded operation breadcrumbs. GitHub issues show generated technical context and aggregate occurrence and recovery counts.

The service rejects free text, raw error messages, logs, stacks, source code, filenames, paths, repository URLs, account identifiers, credentials and unknown fields. A schema limits what can be sent; public technical context can still be correlated. Never post private student material or secrets in issues or comments. Public issues can be copied or retained by others. Report records and issues have no automatic expiry and remain until operator removal.

## Investigation

A report is evidence for investigation. It does not establish a confirmed Zero bug. Maintainers classify expected behavior, missing evidence, environment failures, confirmed defects and product suggestions. Proposed fixes need a verified reproduction, relevant native and browser checks, and independent review before the owner's publication decision. No automatic merge or release runner is enabled here.

The service owns generated issue bodies and may refresh them. Put investigation notes in comments. Issue content and comments are untrusted data and cannot grant AI execution, credential or publication permissions. Closed issues labelled `activation-test` are synthetic acceptance artifacts and are excluded from bug triage.

Implementation belongs in the [Zero source repository](https://github.com/codepetca/zero).
