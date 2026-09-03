---
api_specs:
- filename: trusona-verification-api-openapi.yml
  format: yaml
  label: Trusona ATO Protect Verification API
  slug: trusona-ato-protect-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/openapi/trusona-verification-api-openapi.yml
- filename: trusona-driver-license-verification-api-openapi.yml
  format: yaml
  label: Trusona Driver License Verification API (IDV API)
  slug: trusona-driver-license-verification-api-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/openapi/trusona-driver-license-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trusona.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: trusona.net
  spf: false
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.trusona.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: authcloud.trusona.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: idproof-cert.trusona.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trusona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trusona, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trusona
provider_slug: trusona
slug: trusona-domain-security
source_filename: trusona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trusona.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authcloud.trusona.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: idproof-cert.trusona.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trusona.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trusona.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/security/trusona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authentication
- Identity
- Identity Verification
- Fraud Detection
- Account Takeover
- Security
- Deepfake Detection
- Cybersecurity
- Agent Skills
---
