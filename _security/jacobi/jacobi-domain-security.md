---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jacobistrategies.com
  spf: true
hosts:
- cert_expires: Oct 28 10:36:43 2026 GMT
  host: www.jacobistrategies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:56:44 2026 GMT
  host: app.jacobistrategies.com
  hsts: false
  https: true
  note: application host (login); no Strict-Transport-Security header on the 302 root response
  tls_version: TLSv1.3
- cert_expires: Sep 25 08:12:17 2026 GMT
  host: docs.jacobistrategies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: login-gated BookStack knowledge center
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jacobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jacobi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jacobi
provider_slug: jacobi
slug: jacobi-domain-security
source_filename: jacobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jacobistrategies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:36:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.jacobistrategies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:56:44 2026 GMT\n  hsts: false\n  note: application host (login); no Strict-Transport-Security header on the 302 root response\n- host: docs.jacobistrategies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:12:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: login-gated BookStack knowledge center\ndomains:\n- domain: jacobistrategies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jacobi/refs/heads/main/security/jacobi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- investment-management
- portfolio-analytics
- asset-allocation
- multi-asset
- wealth-management
- fintech
- risk-analytics
- model-portfolios
- ocio
- financial-services
- saas
---
