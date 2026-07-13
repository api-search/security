---
api_specs:
- filename: qualtrics-api-openapi-3.0.json
  format: json
  label: Qualtrics REST API
  slug: qualtrics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-api-openapi-3.0.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: qualtrics.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.qualtrics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 13:58:19 2026 GMT
  host: api.qualtrics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: yourdatacenterid.qualtrics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualtrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualtrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Qualtrics
provider_slug: qualtrics
slug: qualtrics-domain-security
source_filename: qualtrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualtrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.qualtrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:58:19 2026 GMT\n  hsts: false\n- host: yourdatacenterid.qualtrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qualtrics.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/security/qualtrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Experience Management
- Surveys
- Customer Experience
- Employee Experience
- Market Research
- XM
- REST API
---
