---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wealthkernel.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wealthkernel.io
  spf: false
hosts:
- cert_expires: Oct 14 20:54:56 2026 GMT
  host: www.wealthkernel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 00:10:16 2026 GMT
  host: docs.wealthkernel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.wealthkernel.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealthkernel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WealthKernel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WealthKernel
provider_slug: wealthkernel
slug: wealthkernel-domain-security
source_filename: wealthkernel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealthkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wealthkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:10:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wealthkernel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wealthkernel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wealthkernel.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthkernel/refs/heads/main/security/wealthkernel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Investing
- Wealth Management
- Brokerage
- Custody
- Fintech
- Investment API
- Embedded Finance
- ISA
- SIPP
- Banking as a Service
- United Kingdom
- Europe
---
