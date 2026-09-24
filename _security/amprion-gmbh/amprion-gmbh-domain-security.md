---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amprion.net
  spf: true
hosts:
- cert_expires: Dec  9 07:27:09 2026 GMT
  host: www.amprion.net
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amprion Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amprion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amprion
provider_slug: amprion-gmbh
slug: amprion-gmbh-domain-security
source_filename: amprion-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amprion.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 07:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: amprion.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amprion-gmbh/refs/heads/main/security/amprion-gmbh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Transmission
- Grid
- Infrastructure
---
