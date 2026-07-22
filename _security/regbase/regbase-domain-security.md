---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regbase.com
  spf: true
hosts:
- cert_expires: Oct  8 18:22:25 2026 GMT
  host: regbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Regbase
provider_slug: regbase
slug: regbase-domain-security
source_filename: regbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: regbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regbase/refs/heads/main/security/regbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Regulatory Intelligence
- Compliance
- RegTech
- Legal Technology
- GovTech
- Regulatory Monitoring
- Artificial Intelligence
---
