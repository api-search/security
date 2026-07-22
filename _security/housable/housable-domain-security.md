---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: housable.com
  spf: true
hosts:
- cert_expires: Aug 24 00:31:23 2026 GMT
  host: housable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Housable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Housable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Housable
provider_slug: housable
slug: housable-domain-security
source_filename: housable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: housable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:31:23 2026 GMT\n  hsts: false\ndomains:\n- domain: housable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housable/refs/heads/main/security/housable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- ADU
- Accessory Dwelling Units
- Real Estate
- PropTech
- Construction
- Property Management
- Housing
- California
---
