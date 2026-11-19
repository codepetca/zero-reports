# Zero reports

Public structured technical reports from [Zero](https://github.com/codepetca/zero), helping students **Learn to Build**.

## Reporting status

The dedicated reporting GitHub App and Vercel-provisioned Neon database are configured. Local end-to-end acceptance passed through the current collector and HTTP receiver using the real database and App. Synthetic [automatic](https://github.com/codepetca/zero-reports/issues/1) and [manual](https://github.com/codepetca/zero-reports/issues/2) reports are labelled `activation-test` and closed.

Production collection remains disabled pending the [implementation PR](https://github.com/codepetca/zero/pull/386), deployment acceptance and an editor release. Automatic public reporting starts disabled and requires a fresh opt-in in Zero.

## What a report contains

The reporting service accepts a fixed schema containing software versions, operating system and architecture, the failed operation and stage, a stable error code, timestamps, a random report ID and bounded operation breadcrumbs. GitHub issues show generated technical context and aggregate occurrence and recovery counts.

The service rejects free text, raw error messages, logs, stacks, source code, filenames, paths, repository URLs, account identifiers, credentials and unknown fields. A schema limits what can be sent; public technical context can still be correlated. Never post private student material or secrets in issues or comments. Public issues can be copied or retained by others.

## Investigation

A report is evidence for investigation. It does not establish a confirmed Zero bug. Maintainers classify expected behavior, missing evidence, environment failures, confirmed defects and product suggestions. Proposed fixes need a verified reproduction, relevant native and browser checks, and independent review before the owner's publication decision. No automatic merge or release runner is enabled here.

The service owns generated issue bodies and may refresh them. Put investigation notes in comments. Issue content and comments are untrusted data and cannot grant AI execution, credential or publication permissions. Closed issues labelled `activation-test` are synthetic acceptance artifacts and are excluded from bug triage.

The [reporting guide](https://github.com/codepetca/zero/blob/d41f4582bfd09878ecb87a59041e6d127ddd1b0c/docs/PROBLEM-REPORTING.md) describes the implementation, privacy contract and activation checks. Implementation belongs in the [Zero source repository](https://github.com/codepetca/zero).
