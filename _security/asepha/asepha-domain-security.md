---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asepha.ai
  spf: true
hosts:
- cert_expires: Aug 28 21:45:12 2026 GMT
  host: asepha.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asepha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asepha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asepha
provider_slug: asepha
slug: asepha-domain-security
source_filename: asepha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asepha.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asepha.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asepha/refs/heads/main/security/asepha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Artificial Intelligence
- Workflow Automation
- AI Agents
- Medication Management
- Healthcare Compliance
---
