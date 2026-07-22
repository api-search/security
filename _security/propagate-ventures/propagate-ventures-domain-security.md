---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: propagateag.com
  spf: true
hosts:
- cert_expires: Sep  7 19:19:51 2026 GMT
  host: www.propagateag.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propagate Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propagate Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Propagate Ventures
provider_slug: propagate-ventures
slug: propagate-ventures-domain-security
source_filename: propagate-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propagateag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:19:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: propagateag.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propagate-ventures/refs/heads/main/security/propagate-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Agriculture
- Agroforestry
- Regenerative Agriculture
- Climate
- Farm Software
- SaaS
- Sustainability
---
