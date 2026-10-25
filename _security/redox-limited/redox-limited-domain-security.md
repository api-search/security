---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: redox.com
  spf: true
hosts:
- cert_expires: Dec 27 01:40:29 2026 GMT
  host: redox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Redox Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Redox
provider_slug: redox-limited
slug: redox-limited-domain-security
source_filename: redox-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 01:40:29 2026 GMT\n  hsts: false\ndomains:\n- domain: redox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redox-limited/refs/heads/main/security/redox-limited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Chemicals
- Distribution
- Ingredients
- Supply Chain
- Australia
---
