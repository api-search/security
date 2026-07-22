---
api_specs:
- filename: verifiable-openapi-original.json
  format: json
  label: Verifiable API
  slug: verifiable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verifiable/refs/heads/main/openapi/verifiable-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verifiable.com
  spf: true
hosts:
- cert_expires: Oct  3 18:30:44 2026 GMT
  host: verifiable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: discovery.verifiable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: discovery-staging.verifiable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verifiable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verifiable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verifiable
provider_slug: verifiable
slug: verifiable-domain-security
source_filename: verifiable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verifiable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:30:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discovery.verifiable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discovery-staging.verifiable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verifiable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verifiable/refs/heads/main/security/verifiable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Credentialing
- Provider Data
- Primary Source Verification
- Compliance
- Monitoring
- API
---
