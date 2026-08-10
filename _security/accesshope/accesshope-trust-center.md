---
certifications:
- HITRUST CSF r2
- SOC 2 Type I
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Accesshope Trust Center
name_suffix: Trust Center
overview: AccessHope maintains a public trust center documenting HITRUST CSF r2, SOC 2 Type I, and SOC 2 Type II compliance.
provider_name: AccessHope
provider_slug: accesshope
slug: accesshope-trust-center
source_filename: accesshope-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nprobe: true\nurl: https://trust.myaccesshope.org/\nplatform: Thoropass (formerly Laika) hosted Trust Center\ntitle: Trust Center\n\n# The trust center is a first-party subdomain of myaccesshope.org that AccessHope\n# operates through Thoropass. The served HTML is an 814-byte SPA shell; the content\n# (frameworks, controls, documents, subprocessors) loads from Thoropass's AppSync\n# GraphQL API, which rejects anonymous callers. Document downloads sit behind an\n# email + NDA access-group gate. So the trust center EXISTS and is first-party, but\n# its contents are not machine-readable to an anonymous client.\nreadable_anonymously: false\ngating: email + NDA access group (Thoropass access-group flow) for documents\n\ncertifications:\n- HITRUST CSF r2\n- SOC 2 Type I\n- SOC 2 Type II\ncertifications_source: >-\n  Named in AccessHope's own press release, not read off the trust center — the trust\n  center payload is auth-gated. See conformance/accesshope-conformance.yml.\n\
  \nevidence:\n- source: https://trust.myaccesshope.org/\n  http_status: 200\n  content_type: text/html; charset=utf-8\n  size: 814\n  server: gunicorn via CloudFront\n  keywords: [trust center]\n  note: >-\n    Distinct DNS record — a control host (zzz-nope-control.myaccesshope.org) does not\n    resolve, so this is not a wildcard soft-200.\n- source: https://laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js\n  http_status: 200\n  note: Thoropass trust-center SPA bundle referenced by the page\n- source: https://fhovr7cwmfgebommmcztmsw5ze.appsync-api.us-east-1.amazonaws.com/graphql\n  http_status: 401\n  note: >-\n    Anonymous PublicTrustCenterData query returned UnauthorizedException; trust center\n    contents cannot be harvested without credentials.\n- source: https://security.myaccesshope.org/\n  http_status: 0\n  note: does not resolve\n- source: https://www.myaccesshope.org/compliance\n  http_status: 404\n\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://trust.myaccesshope.org/\n\
  \  http_status: 200\n  content_type: text/html; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accesshope/refs/heads/main/security/accesshope-trust-center.yml
summary_line: HITRUST CSF r2, SOC 2 Type I, SOC 2 Type II
tags:
- Company
- Healthcare
- Oncology
- Cancer Care
- Employee Benefits
- Health Benefits
- Digital Health
- Telehealth
- Second Opinion
- Employer Health
trust_url: https://trust.myaccesshope.org/
---
