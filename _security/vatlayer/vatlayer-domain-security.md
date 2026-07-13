---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vatlayer.com
  spf: true
hosts:
- cert_expires: Oct  1 18:12:57 2026 GMT
  host: vatlayer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VATlayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VATlayer
provider_slug: vatlayer
slug: vatlayer-domain-security
source_filename: vatlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:12:57 2026 GMT\n  hsts: false\ndomains:\n- domain: vatlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatlayer/refs/heads/main/security/vatlayer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Validation
- Public APIs
---
