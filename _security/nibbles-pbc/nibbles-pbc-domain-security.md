---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nibbles.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: nibbles.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nibbles Pbc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nibbles PBC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nibbles PBC
provider_slug: nibbles-pbc
slug: nibbles-pbc-domain-security
source_filename: nibbles-pbc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nibbles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nibbles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nibbles-pbc/refs/heads/main/security/nibbles-pbc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pet
- Insurance
- Financial Services
- Credit Card
- Consumer
- Public Benefit Company
- Rewards
---
