---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: semantha.de
  spf: true
hosts:
- cert_expires: Sep  6 07:26:12 2026 GMT
  host: www.semantha.de
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Thingsthinking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thingsthinking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thingsthinking
provider_slug: thingsthinking
slug: thingsthinking-domain-security
source_filename: thingsthinking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.semantha.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 07:26:12 2026 GMT\n  hsts: false\ndomains:\n- domain: semantha.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingsthinking/refs/heads/main/security/thingsthinking-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Semantic AI
- Natural Language Processing
- Document Analysis
- Enterprise Search
- Contract Analysis
- Text Analytics
- Machine Learning
- Compliance
- REST API
- Germany
---
