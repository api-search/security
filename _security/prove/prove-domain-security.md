---
api_specs:
- filename: prove-auth-api-openapi.yml
  format: yaml
  label: Prove Auth API
  slug: prove-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-auth-api-openapi.yml
- filename: prove-authentication-api-openapi.yml
  format: yaml
  label: Prove Authentication API
  slug: prove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-authentication-api-openapi.yml
- filename: prove-domain-api-openapi.yml
  format: yaml
  label: Prove Domain API
  slug: prove-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-domain-api-openapi.yml
- filename: prove-identity-api-openapi.yml
  format: yaml
  label: Prove Identity API
  slug: prove-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-api-openapi.yml
- filename: prove-identity-verification-api-openapi.yml
  format: yaml
  label: Prove Identity Verification API
  slug: prove-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-verification-api-openapi.yml
- filename: prove-pre-fill-api-openapi.yml
  format: yaml
  label: Prove Pre-Fill API
  slug: prove-pre-fill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-pre-fill-api-openapi.yml
- filename: prove-trust-score-api-openapi.yml
  format: yaml
  label: Prove Trust Score API
  slug: prove-trust-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-trust-score-api-openapi.yml
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
