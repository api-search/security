---
api_specs:
- filename: swift-swiftref-api-openapi.yml
  format: yaml
  label: SwiftRef API
  slug: swiftref-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swift/refs/heads/main/openapi/swift-swiftref-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swift.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developer.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWIFT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SWIFT
provider_slug: swift
slug: swift-domain-security
source_filename: swift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: developer.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: api.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift/refs/heads/main/security/swift-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
---
