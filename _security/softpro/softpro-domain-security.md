---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: softprocorp.com
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: www.softprocorp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 05:17:08 2026 GMT
  host: info.softprocorp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Softpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoftPro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SoftPro
provider_slug: softpro
slug: softpro-domain-security
source_filename: softpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softprocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: info.softprocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: softprocorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softpro/refs/heads/main/security/softpro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Title Insurance
- Escrow
- Real Estate Closing
- Settlement
- Title Production
- SoftPro 360
- Integration Marketplace
- Partner API
---
