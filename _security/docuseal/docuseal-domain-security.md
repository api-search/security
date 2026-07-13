---
api_specs:
- filename: docuseal-docuseal-api-openapi.yml
  format: yaml
  label: DocuSeal REST API
  slug: docuseal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/openapi/docuseal-docuseal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docuseal.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: docuseal.eu
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.docuseal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 20:49:36 2026 GMT
  host: api.docuseal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 18:17:14 2026 GMT
  host: api.docuseal.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docuseal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocuSeal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DocuSeal
provider_slug: docuseal
slug: docuseal-domain-security
source_filename: docuseal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docuseal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.docuseal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:49:36 2026 GMT\n  hsts: null\n- host: api.docuseal.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:17:14 2026 GMT\n  hsts: null\ndomains:\n- domain: docuseal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: docuseal.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/security/docuseal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Signing
- eSignature
- Electronic Signature
- Document Management
- PDF
- Templates
- Open Source
- Webhooks
- Embedding
---
