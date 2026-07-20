---
api_specs:
- filename: hopae-inc-hconnect-openapi-original.json
  format: json
  label: Hopae hConnect API
  slug: hopae-inc-hconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/openapi/hopae-inc-hconnect-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hopae.com
  spf: true
hosts:
- cert_expires: Aug 28 06:37:05 2026 GMT
  host: hopae.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: sandbox.api.hopae.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopae Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hopae, Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hopae, Inc.
provider_slug: hopae-inc
slug: hopae-inc-domain-security
source_filename: hopae-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hopae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 06:37:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.api.hopae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hopae.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/security/hopae-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity
- Identity Verification
- Digital Identity
- eID
- Verifiable Credentials
- Authentication
- OpenID Connect
- eIDAS
- KYC
---
