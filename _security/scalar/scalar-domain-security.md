---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalar.com
  spf: true
hosts:
- cert_expires: Oct  5 22:09:48 2026 GMT
  host: scalar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 06:36:56 2026 GMT
  host: guides.scalar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalar
provider_slug: scalar
slug: scalar-domain-security
source_filename: scalar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scalar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:09:48 2026 GMT\n  hsts: false\n- host: guides.scalar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:36:56 2026 GMT\n  hsts: false\ndomains:\n- domain: scalar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalar/refs/heads/main/security/scalar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Client
- API Documentation
- API References
- Code Generation
- Developer Tools
- OpenAPI
- Registry
- SDKs
- Swagger
---
