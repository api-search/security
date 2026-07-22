---
api_specs:
- filename: smile-identity-v3-openapi.json
  format: json
  label: Smile ID V3 API
  slug: smile-id-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usesmileid.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smileidentity.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: usesmileid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:11:34 2026 GMT
  host: docs.usesmileid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:29:57 2026 GMT
  host: api.smileidentity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smile Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smile Identity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smile Identity
provider_slug: smile-identity
slug: smile-identity-domain-security
source_filename: smile-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usesmileid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.usesmileid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:11:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smileidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:29:57 2026 GMT\n  hsts: null\ndomains:\n- domain: usesmileid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smileidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/security/smile-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Verification
- KYC
- KYB
- Biometrics
- Liveness Detection
- Document Verification
- AML
- Fraud Prevention
- Compliance
- Onboarding
- Africa
---
