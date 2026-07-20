---
api_specs:
- filename: eigenpal-openapi-original.json
  format: json
  label: Eigenpal API
  slug: eigenpal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eigenpal/refs/heads/main/openapi/eigenpal-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eigenpal.com
  spf: false
hosts:
- cert_expires: Oct 10 00:03:26 2026 GMT
  host: www.eigenpal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 12:59:59 2026 GMT
  host: docs.eigenpal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 00:03:26 2026 GMT
  host: studio.eigenpal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eigenpal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eigenpal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Eigenpal
provider_slug: eigenpal
slug: eigenpal-domain-security
source_filename: eigenpal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eigenpal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:03:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.eigenpal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: studio.eigenpal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:03:26 2026 GMT\n  hsts: null\ndomains:\n- domain: eigenpal.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigenpal/refs/heads/main/security/eigenpal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Document Processing
- Artificial Intelligence
- Workflow Automation
- Machine Learning
- Data Extraction
- OCR
- Developer Tools
- Enterprise
---
