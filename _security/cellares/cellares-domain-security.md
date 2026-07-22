---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cellares.com
  spf: true
hosts:
- cert_expires: Aug 29 07:56:37 2026 GMT
  host: cellares.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cellares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellares, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cellares
provider_slug: cellares
slug: cellares-domain-security
source_filename: cellares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cellares.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellares/refs/heads/main/security/cellares-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cell Therapy
- Biotechnology
- Manufacturing
- Life Sciences
- Automation
- Quality Control
---
