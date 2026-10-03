---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aras.com
  spf: true
hosts:
- cert_expires: Nov 23 17:16:09 2026 GMT
  host: aras.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aras, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aras
provider_slug: aras
slug: aras-domain-security
source_filename: aras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 17:16:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aras.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aras/refs/heads/main/security/aras-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- PLM
- Digital Thread
- Low-Code Development
- PLM Software
- Cloud Platform
- AI-Ready
- Industry Solutions
---
