---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revelaihealth.com
  spf: true
hosts:
- cert_expires: Sep 20 03:15:13 2026 GMT
  host: revelaihealth.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revel Ai Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revel Ai Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revel Ai Health
provider_slug: revel-ai-health
slug: revel-ai-health-domain-security
source_filename: revel-ai-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revelaihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: revelaihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revel-ai-health/refs/heads/main/security/revel-ai-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Conversational AI
- Value-Based Care
- Orthopedics
- Digital Health
---
