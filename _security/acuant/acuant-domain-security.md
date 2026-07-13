---
api_specs:
- filename: acuant-assureid-connect-openapi.yml
  format: yaml
  label: Acuant AssureID Connect API
  slug: assureid-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-assureid-connect-openapi.yml
- filename: acuant-frm-openapi.yml
  format: yaml
  label: Acuant FRM Face Recognition API
  slug: frm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-frm-openapi.yml
- filename: acuant-passive-liveness-openapi.yml
  format: yaml
  label: Acuant Passive Liveness API
  slug: passive-liveness
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-passive-liveness-openapi.yml
- filename: acuant-acas-openapi.yml
  format: yaml
  label: Acuant ACAS (Cloud Authentication Service) API
  slug: acas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-acas-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuant.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assureid.net
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.acuant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: services.assureid.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: frm.acuant.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acuant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acuant, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acuant
provider_slug: acuant
slug: acuant-domain-security
source_filename: acuant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acuant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.assureid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: frm.acuant.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: acuant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: assureid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/security/acuant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Document Authentication
- Biometrics
- Face Matching
- Liveness Detection
- KYC
- AML
- ID Capture
---
