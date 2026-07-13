---
api_specs:
- filename: at-bay-partner-api-openapi.yml
  format: yaml
  label: At-Bay Partner API
  slug: at-bay-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/openapi/at-bay-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: at-bay.com
  spf: true
hosts:
- cert_expires: Sep 15 05:51:01 2026 GMT
  host: www.at-bay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:24:27 2026 GMT
  host: developers.at-bay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 09:31:08 2026 GMT
  host: api.at-bay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: At Bay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for At-Bay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: At-Bay
provider_slug: at-bay
slug: at-bay-domain-security
source_filename: at-bay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.at-bay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:51:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.at-bay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:24:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.at-bay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:31:08 2026 GMT\n  hsts: null\ndomains:\n- domain: at-bay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/security/at-bay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Cyber Insurance
- InsurSec
- Insurtech
- Tech E&O
- Professional Liability
- MPL
- Managed Detection And Response
- MDR
- Security Monitoring
- Email Security
- Endpoint Security
- Incident Response
- Brokers
- Quoting
- Binding
- Policy Lifecycle
- Webhooks
---
