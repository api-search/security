---
api_specs:
- filename: rics-digitalcommunity-api-openapi.json
  format: json
  label: RICS DigitalCommunity API
  slug: rics-digitalcommunity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-digitalcommunity-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rics.org
  spf: true
hosts:
- cert_expires: Sep 24 10:29:07 2026 GMT
  host: www.rics.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: api.rics.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RICS (Royal Institution of Chartered Surveyors), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RICS (Royal Institution of Chartered Surveyors)
provider_slug: rics
slug: rics-domain-security
source_filename: rics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rics.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:29:07 2026 GMT\n  hsts: false\n- host: api.rics.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rics.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/security/rics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United Kingdom
- Industry Body
- Valuation
- Standards
- Surveying
- Property Measurement
- Regulations
- Construction
- PropTech
---
