---
api_specs:
- filename: zayo-openapi-original.yml
  format: yaml
  label: Zayo APIs
  slug: zayo-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zayo.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: developer.zayo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.zayo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zayo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zayo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zayo
provider_slug: zayo
slug: zayo-domain-security
source_filename: zayo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.zayo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: api.zayo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zayo.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/security/zayo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telecommunications
- Networking
- Connectivity
- Fiber
- Infrastructure
- Bandwidth
- Cloud Connectivity
- Ordering
- Ticketing
---
