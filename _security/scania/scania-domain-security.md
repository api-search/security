---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scania.com
  spf: true
hosts:
- cert_expires: Dec  7 06:14:41 2026 GMT
  host: scania.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scania Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scania, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scania
provider_slug: scania
slug: scania-domain-security
source_filename: scania-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scania.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 06:14:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scania.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scania/refs/heads/main/security/scania-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Trucking
- Transportation
- Manufacturing
- Sustainability
---
