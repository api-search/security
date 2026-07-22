---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sands.com
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.sands.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Las Vegas Sands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Las Vegas Sands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Las Vegas Sands
provider_slug: las-vegas-sands
slug: las-vegas-sands-domain-security
source_filename: las-vegas-sands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/las-vegas-sands/refs/heads/main/security/las-vegas-sands-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Casino
- Conventions
- Entertainment
- Hospitality
- Hotels
- Integrated Resorts
- Resorts
- Fortune 500
---
