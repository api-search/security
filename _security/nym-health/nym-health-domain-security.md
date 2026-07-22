---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nym.health
  spf: true
hosts:
- cert_expires: Sep 29 11:08:41 2026 GMT
  host: nym.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nym Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nym Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nym Health
provider_slug: nym-health
slug: nym-health-domain-security
source_filename: nym-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nym.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nym.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nym-health/refs/heads/main/security/nym-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Medical Coding
- Autonomous Coding
- Clinical NLP
- Revenue Cycle
- Health IT
---
