---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: novoic.com
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: novoic.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Novoic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novoic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Novoic
provider_slug: novoic
slug: novoic-domain-security
source_filename: novoic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novoic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: novoic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novoic/refs/heads/main/security/novoic-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- Speech
- Healthcare
- Alzheimers
- Biomarkers
- Machine Learning
- Digital Health
- Neurology
- Cognitive Assessment
---
