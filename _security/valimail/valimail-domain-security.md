---
api_specs:
- filename: valimail-config-openapi-original.yml
  format: yaml
  label: Valimail Configuration API
  slug: valimail-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-config-openapi-original.yml
- filename: valimail-account-openapi-original.yml
  format: yaml
  label: Valimail Account Management API
  slug: valimail-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-account-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valimail.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: valimail-staging.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.valimail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.valimail.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.valimail-staging.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Valimail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valimail, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Valimail
provider_slug: valimail
slug: valimail-domain-security
source_filename: valimail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valimail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.valimail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63113904\n- host: api.valimail-staging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63113904\ndomains:\n- domain: valimail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: valimail-staging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/security/valimail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Authentication
- DMARC
- Email Security
- SPF
- DKIM
- BIMI
- MTA-STS
- Anti-Phishing
- Deliverability
- Cybersecurity
---
