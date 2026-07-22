---
api_specs:
- filename: nitro-software-openapi-original.json
  format: json
  label: Nitro API (Sign + PDF Services)
  slug: nitro-api-sign-pdf-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitro-software/refs/heads/main/openapi/nitro-software-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@gonitro.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gonitro.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gonitro.dev
  spf: false
hosts:
- cert_expires: Oct 17 18:42:53 2026 GMT
  host: developers.gonitro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:41:16 2026 GMT
  host: api.gonitro.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nitro Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nitro Software, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nitro Software
provider_slug: nitro-software
slug: nitro-software-domain-security
source_filename: nitro-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.gonitro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:42:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gonitro.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:41:16 2026 GMT\n  hsts: null\ndomains:\n- domain: gonitro.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@gonitro.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gonitro.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nitro-software/refs/heads/main/security/nitro-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- PDF
- Documents
- eSignature
- Electronic Signature
- Document Management
- Document Intelligence
- OCR
- Data Extraction
- Productivity
---
