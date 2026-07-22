---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eleos.health
  spf: true
hosts:
- cert_expires: Sep  5 17:37:24 2026 GMT
  host: eleos.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eleos Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eleos Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Eleos Health
provider_slug: eleos-health
slug: eleos-health-domain-security
source_filename: eleos-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eleos.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eleos.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eleos-health/refs/heads/main/security/eleos-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Behavioral Health
- Healthcare AI
- Clinical Documentation
- Compliance
- Revenue Cycle Management
- Electronic Health Records
- Community-Based Care
- Mental Health
---
