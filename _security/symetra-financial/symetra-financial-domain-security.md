---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: symetra.com
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.symetra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.symetra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Symetra Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symetra Financial, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Symetra Financial
provider_slug: symetra-financial
slug: symetra-financial-domain-security
source_filename: symetra-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.symetra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\n- host: api.symetra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: symetra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symetra-financial/refs/heads/main/security/symetra-financial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Annuities
- Benefits
- Employee Benefits
- Financial Services
- Insurance
- Life Insurance
- Stop Loss
- Fortune 1000
---
