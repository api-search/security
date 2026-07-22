---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: paradigm.inc
  spf: true
hosts:
- cert_expires: Sep  3 15:28:27 2026 GMT
  host: www.paradigm.inc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paradigm Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paradigm Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Paradigm Health
provider_slug: paradigm-health
slug: paradigm-health-domain-security
source_filename: paradigm-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paradigm.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:28:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paradigm.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradigm-health/refs/heads/main/security/paradigm-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- Clinical Research
- Health Data
- Artificial Intelligence
---
