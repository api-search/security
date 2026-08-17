---
api_specs:
- filename: overview
  format: yaml
  label: Change Healthcare Medical Network API
  slug: change-healthcare-api
  spec_type: Postman
  url: https://www.postman.com/changehealthcare-cdp-dev/workspace/change-healthcare-medical-network-apis/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: changehealthcare.com
  spf: true
- caa:
  - 0 issuemail "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optum.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.changehealthcare.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 00:56:30 2026 GMT
  host: developers.changehealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 05:03:48 2026 GMT
  host: apigw.optum.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Change Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Change Healthcare, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Change Healthcare
provider_slug: change-healthcare
slug: change-healthcare-domain-security
source_filename: change-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.changehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.changehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 00:56:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigw.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: changehealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: optum.com\n  dnssec: true\n  caa:\n  - 0 issuemail \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/change-healthcare/refs/heads/main/security/change-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Technology
- Analytics
- EDI
- Claims
- Eligibility
- Clearinghouse
- Revenue Cycle Management
- Prior Authorization
---
