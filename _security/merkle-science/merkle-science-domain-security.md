---
api_specs:
- filename: merkle-science-kybb-openapi.yml
  format: yaml
  label: Merkle Science KYBB API
  slug: merkle-science-kybb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merkle-science/refs/heads/main/openapi/merkle-science-kybb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: merklescience.com
  spf: true
hosts:
- cert_expires: Oct 16 09:49:47 2026 GMT
  host: merklescience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 01:35:21 2026 GMT
  host: kybb.docs.merklescience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 16:08:29 2026 GMT
  host: api.kybb.app.merklescience.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merkle Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merkle Science, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Merkle Science
provider_slug: merkle-science
slug: merkle-science-domain-security
source_filename: merkle-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merklescience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 09:49:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kybb.docs.merklescience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 01:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kybb.app.merklescience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:08:29 2026 GMT\n  hsts: null\ndomains:\n- domain: merklescience.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merkle-science/refs/heads/main/security/merkle-science-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain Analytics
- Cryptocurrency
- Compliance
- AML
- KYC
- Risk
- Fraud Detection
- Due Diligence
- RegTech
---
