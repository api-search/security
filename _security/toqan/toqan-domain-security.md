---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: toqan.ai
  spf: true
hosts:
- cert_expires: Jan 17 20:44:06 2027 GMT
  host: toqan.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Toqan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toqan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Toqan
provider_slug: toqan
slug: toqan-domain-security
source_filename: toqan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toqan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 20:44:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: toqan.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/toqan/security/toqan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI workspace
- Low‑code automation
- Internal tools
- Knowledge base
- Hospitality
---
