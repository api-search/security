---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epiqglobal.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: access.epiqglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.epiqglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epiq, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Epiq
provider_slug: epiq
slug: epiq-domain-security
source_filename: epiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: access.epiqglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.epiqglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: epiqglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epiq/refs/heads/main/security/epiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- eDiscovery
- Bankruptcy
- Class Action
- Settlement Administration
- Legal Technology
- Case Management
- Document Review
---
