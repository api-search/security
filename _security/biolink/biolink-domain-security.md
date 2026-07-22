---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biolink.com.cn
  spf: false
hosts:
- cert_expires: Aug 18 07:08:28 2026 GMT
  host: biolink.com.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biolink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for biolink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: biolink
provider_slug: biolink
slug: biolink-domain-security
source_filename: biolink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biolink.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:08:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biolink.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolink/refs/heads/main/security/biolink-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Bioprocessing
- Biopharmaceutical
- Biotechnology
- Life Sciences
- Manufacturing
- Single-Use Systems
- China
---
