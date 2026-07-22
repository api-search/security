---
api_specs:
- filename: smallstep-openapi-original.yml
  format: yaml
  label: Smallstep Platform API
  slug: smallstep-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallstep/refs/heads/main/openapi/smallstep-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smallstep.com
  spf: true
hosts:
- cert_expires: Oct 12 05:33:20 2026 GMT
  host: www.smallstep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:39:50 2026 GMT
  host: gateway.smallstep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smallstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmallStep, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SmallStep
provider_slug: smallstep
slug: smallstep-domain-security
source_filename: smallstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smallstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:33:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.smallstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:39:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smallstep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallstep/refs/heads/main/security/smallstep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Certificate Authority
- PKI
- Device Identity
- Zero Trust
- Certificate Management
- mTLS
- ACME
- SSH
- Security
---
