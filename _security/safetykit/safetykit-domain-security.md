---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: safetykit.com
  spf: true
hosts:
- cert_expires: Oct 12 03:33:01 2026 GMT
  host: www.safetykit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:54:28 2026 GMT
  host: docs.safetykit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.safetykit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safetykit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SafetyKit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SafetyKit
provider_slug: safetykit
slug: safetykit-domain-security
source_filename: safetykit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.safetykit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.safetykit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.safetykit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: safetykit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safetykit/refs/heads/main/security/safetykit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Trust and Safety
- Fraud Detection
- Content Moderation
- Risk
- AI Agents
- Compliance
---
