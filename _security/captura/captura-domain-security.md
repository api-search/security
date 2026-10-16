---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: captura.io
  spf: true
hosts:
- cert_expires: Nov 10 14:18:07 2026 GMT
  host: captura.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Captura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Captura
provider_slug: captura
slug: captura-domain-security
source_filename: captura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: captura.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:18:07 2026 GMT\n  hsts: false\ndomains:\n- domain: captura.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captura/refs/heads/main/security/captura-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Photography
- SaaS
- Workflow
- Imaging
---
