---
api_specs:
- filename: listen-labs-study-data-openapi.json
  format: json
  label: Listen Labs Public API — Study Data
  slug: study-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/openapi/listen-labs-study-data-openapi.json
- filename: listen-labs-v2-openapi.yml
  format: yaml
  label: Listen Labs Public API v2
  slug: v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/openapi/listen-labs-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: listenlabs.ai
  spf: true
hosts:
- cert_expires: Aug 24 14:41:53 2026 GMT
  host: www.listenlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 04:42:07 2026 GMT
  host: docs.listenlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 13:01:07 2026 GMT
  host: listenlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listen Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listen Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Listen Labs
provider_slug: listen-labs
slug: listen-labs-domain-security
source_filename: listen-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.listenlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:41:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.listenlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:42:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: listenlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: listenlabs.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/security/listen-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Market Research
- Customer Research
- User Interviews
- Surveys
- Qualitative Research
- Voice AI
- Insights
- Agents
---
