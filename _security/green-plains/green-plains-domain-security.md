---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gpreinc.com
  spf: true
hosts:
- cert_expires: Sep 27 22:03:24 2026 GMT
  host: www.gpreinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Plains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Plains, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Green Plains
provider_slug: green-plains
slug: green-plains-domain-security
source_filename: green-plains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gpreinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:03:24 2026 GMT\n  hsts: false\ndomains:\n- domain: gpreinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-plains/refs/heads/main/security/green-plains-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biofuel
- Ethanol
- Agriculture
- Energy
- Fortune 1000
---
