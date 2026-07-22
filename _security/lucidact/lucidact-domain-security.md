---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lucidact.com
  spf: true
hosts:
- cert_expires: Oct  3 18:45:15 2026 GMT
  host: lucidact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucidact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LucidAct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LucidAct
provider_slug: lucidact
slug: lucidact-domain-security
source_filename: lucidact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucidact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:45:15 2026 GMT\n  hsts: false\ndomains:\n- domain: lucidact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidact/refs/heads/main/security/lucidact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Care Management
- Artificial Intelligence
- Clinical Workflow
---
