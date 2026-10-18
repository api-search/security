---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: charterup.com
  spf: true
hosts:
- cert_expires: Dec 13 14:23:03 2026 GMT
  host: www.charterup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charterup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charterup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Charterup
provider_slug: charterup
slug: charterup-domain-security
source_filename: charterup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charterup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 14:23:03 2026 GMT\n  hsts: false\ndomains:\n- domain: charterup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charterup/refs/heads/main/security/charterup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Transportation
- On-Demand
- Bus
- Software-as-a-Service
---
