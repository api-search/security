---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: casetext.com
  spf: true
hosts:
- cert_expires: Sep 11 08:00:07 2026 GMT
  host: casetext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casetext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casetext, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Casetext
provider_slug: casetext
slug: casetext-domain-security
source_filename: casetext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: casetext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 08:00:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: casetext.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casetext/refs/heads/main/security/casetext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Legal Tech
- Legal Research
- Case Law
- Legal AI
- Generative AI
- CoCounsel
- Parallel Search
- AllSearch
- Compose
- SmartCite
- Document Review
- Contract Analysis
- Deposition Preparation
- Thomson Reuters
---
