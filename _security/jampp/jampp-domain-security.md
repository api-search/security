---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jampp.com
  spf: true
hosts:
- cert_expires: Oct  1 17:15:22 2026 GMT
  host: jampp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: developers.jampp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: reporting-api.jampp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jampp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jampp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jampp
provider_slug: jampp
slug: jampp-domain-security
source_filename: jampp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jampp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.jampp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\n- host: reporting-api.jampp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jampp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jampp/refs/heads/main/security/jampp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Mobile
- Analytics
- Reporting
- GraphQL
- Demand-Side Platform
- App Marketing
- Attribution
---
