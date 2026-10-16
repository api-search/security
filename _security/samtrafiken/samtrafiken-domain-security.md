---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: samtrafiken.se
  spf: true
hosts:
- cert_expires: Nov 30 21:50:19 2026 GMT
  host: samtrafiken.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Samtrafiken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Samtrafiken, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Samtrafiken
provider_slug: samtrafiken
slug: samtrafiken-domain-security
source_filename: samtrafiken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: samtrafiken.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 21:50:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: samtrafiken.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samtrafiken/refs/heads/main/security/samtrafiken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transport
- OpenData
- Sweden
- Collaboration
---
