---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: entrata.com
  spf: true
hosts:
- cert_expires: Aug 17 04:31:10 2026 GMT
  host: www.entrata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: docs.entrata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your_domain.entrata.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''your_domain'
kind: domain-security
layout: security
method: probed
name: Entrata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entrata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Entrata
provider_slug: entrata
slug: entrata-domain-security
source_filename: entrata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entrata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:31:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.entrata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: your_domain.entrata.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''your_domain'\n  hsts: null\ndomains:\n- domain: entrata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entrata/refs/heads/main/security/entrata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Management
- Multifamily Housing
- Real Estate
- Resident Management
- Leasing
- Maintenance
- Payments
- Accounting
---
