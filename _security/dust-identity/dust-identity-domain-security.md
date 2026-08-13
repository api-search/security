---
api_specs:
- filename: dust-identity-apid-openapi.yml
  format: yaml
  label: DUST API
  slug: dust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/openapi/dust-identity-apid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dustidentity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dustid.io
  spf: false
hosts:
- cert_expires: Oct 28 03:49:25 2026 GMT
  host: www.dustidentity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: docs.dustid.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: apid.dustid.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dust Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dust Identity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dust Identity
provider_slug: dust-identity
slug: dust-identity-domain-security
source_filename: dust-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dustidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 03:49:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dustid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\n- host: apid.dustid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dustidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dustid.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/security/dust-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Identity
- Supply Chain
- Traceability
- Provenance
- Anti-Counterfeiting
- Asset Tracking
- Aerospace and Defense
- Manufacturing
- Security
---
