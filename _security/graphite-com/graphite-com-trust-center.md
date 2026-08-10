---
api_specs:
- filename: graphite-com-authentication-api-openapi.yml
  format: yaml
  label: Graphite Authentication API
  slug: graphite-com-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-authentication-api-openapi.yml
- filename: graphite-com-github-app-api-openapi.yml
  format: yaml
  label: Graphite GitHub App API
  slug: graphite-com-github-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-github-app-api-openapi.yml
- filename: graphite-com-merge-queue-api-openapi.yml
  format: yaml
  label: Graphite Merge Queue API
  slug: graphite-com-merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-merge-queue-api-openapi.yml
- filename: graphite-com-stacks-api-openapi.yml
  format: yaml
  label: Graphite Stacks API
  slug: graphite-com-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-stacks-api-openapi.yml
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Graphite Com Trust Center
name_suffix: Trust Center
overview: Graphite maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Graphite
provider_slug: graphite-com
slug: graphite-com-trust-center
source_filename: graphite-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nprobe_result: >-\n  probe-security-programs.py returned trust=none — trust.graphite.com does not\n  resolve, and /trust, /security and /compliance on graphite.com all return 404.\n  The trust center was found instead in Graphite's own documentation, which\n  points at the parent company's trust center.\nurl: https://trust.cursor.com\noperated_by: Anysphere (Cursor) — Graphite's parent company since December 2025\nown_domain_trust_center: false\ncertifications:\n- SOC 2 Type II\ncompliance_claims:\n- claim: SOC 2 Type II\n  detail: >-\n    Audited against the AICPA trust services criteria across security,\n    availability, processing integrity, confidentiality and privacy, evaluating\n    the operating effectiveness of controls over a period (typically six months\n    or more) rather than at a point in time.\n  report_request: via https://trust.cursor.com\n  source: https://graphite.com/docs/privacy-and-security\n- claim:\
  \ Continuous penetration testing\n  detail: '\"We also continuously pen test.\"'\n  source: https://graphite.com/docs/privacy-and-security\nenterprise:\n  github_enterprise_server: https://graphite.com/docs/github-enterprise-server\n  vendor_due_diligence: >-\n    Graphite positions the SOC 2 Type II report as the artifact that streamlines\n    enterprise vendor due diligence.\nevidence:\n- source: https://graphite.com/docs/privacy-and-security\n  keywords: [soc 2 type ii, aicpa, pen test, trust center, encryption, aes-256-cbc]\n- source: https://trust.cursor.com\n  http_status: 200\n  note: >-\n    JavaScript application; an anonymous fetch returns only the title \"Cursor\n    Trust Center\". The named certifications above are taken from Graphite's own\n    documentation, not scraped from this page.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://graphite-58cc94ce.mintlify.dev/docs/privacy-and-security.md', http_status: 200}\n  - {url: 'https://trust.cursor.com', http_status:\
  \ 200}\n  - {url: 'https://trust.graphite.com/', http_status: null, note: DNS does not resolve}\n  - {url: 'https://graphite.com/trust', http_status: 404}\n  - {url: 'https://graphite.com/security', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/security/graphite-com-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
trust_url: https://trust.cursor.com
---
