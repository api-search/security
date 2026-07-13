---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vatapi.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: vatapi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: eu.vatapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VAT API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VAT API
provider_slug: vatapi
slug: vatapi-domain-security
source_filename: vatapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\n- host: eu.vatapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vatapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatapi/refs/heads/main/security/vatapi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- VAT
- Tax
- EU
- UK
- Compliance
- Invoice
- VIES
- Business Verification
---
