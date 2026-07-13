---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: taxnexus.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: taxnexus.dev
  spf: false
hosts:
- cert_expires: Aug 22 01:25:18 2026 GMT
  host: taxnexus.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: taxnexus.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Taxnexus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaxNexus, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TaxNexus
provider_slug: taxnexus
slug: taxnexus-domain-security
source_filename: taxnexus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taxnexus.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 01:25:18 2026 GMT\n  hsts: null\n- host: taxnexus.dev\n  https: false\ndomains:\n- domain: taxnexus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: taxnexus.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxnexus/refs/heads/main/security/taxnexus-domain-security.yml
summary_line: TLSv1.2
tags:
- Tax
- Cannabis
- Sales Tax
- Tax Compliance
- Excise Tax
- FinTech
- Cannabis Industry
---
