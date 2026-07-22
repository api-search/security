---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yanyin.tech
  spf: true
hosts:
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: yanyin.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yanyin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yanyin Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yanyin Technology
provider_slug: yanyin
slug: yanyin-domain-security
source_filename: yanyin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yanyin.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yanyin.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yanyin/refs/heads/main/security/yanyin-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Life Sciences
- Artificial Intelligence
- Research
- Electronic Lab Notebook
- LIMS
- SaaS
- China
---
