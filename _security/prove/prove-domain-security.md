---
api_specs:
- filename: prove-openapi.yml
  format: yaml
  label: Prove Identity Verification (v3 Flows)
  slug: identity-verification-v3-flows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-openapi.yml
- filename: prove-openapi.yml
  format: yaml
  label: Prove Trust Score (Unified Authentication)
  slug: trust-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-openapi.yml
- filename: prove-openapi.yml
  format: yaml
  label: Prove Pre-Fill (Identity Discovery)
  slug: pre-fill
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-openapi.yml
- filename: prove-openapi.yml
  format: yaml
  label: Prove Auth
  slug: auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-openapi.yml
- filename: prove-openapi.yml
  format: yaml
  label: Prove Identity Manager
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prove.com
  spf: true
hosts:
- cert_expires: Sep 29 04:34:56 2026 GMT
  host: www.prove.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 10:00:11 2026 GMT
  host: developer.prove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.prove.com
  https: false
kind: domain-security
layout: security
method: probed
name: Prove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prove, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prove
provider_slug: prove
slug: prove-domain-security
source_filename: prove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:34:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.prove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:00:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prove.com\n  https: false\ndomains:\n- domain: prove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/security/prove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Authentication
- Phone Intelligence
- KYC
- Fraud Prevention
---
