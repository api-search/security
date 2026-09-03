---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vendelux.com
  spf: true
hosts:
- cert_expires: Oct 24 06:46:52 2026 GMT
  host: vendelux.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vendelux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vendelux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vendelux
provider_slug: vendelux
slug: vendelux-domain-security
source_filename: vendelux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vendelux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 06:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: vendelux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendelux/refs/heads/main/security/vendelux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Intelligence
- Event Marketing
- B2B Events
- Marketing Intelligence
- Sales Intelligence
- Event Data
- CRM Integration
- Demand Generation
- Field Marketing
- Conference Data
- Company
---
