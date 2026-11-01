---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ap2.com
  spf: true
hosts:
- cert_expires: Dec  5 23:03:04 2026 GMT
  host: www.ap2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: American Pathology Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Pathology Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: American Pathology Partners
provider_slug: american-pathology-partners
slug: american-pathology-partners-domain-security
source_filename: american-pathology-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ap2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:03:04 2026 GMT\n  hsts: false\ndomains:\n- domain: ap2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/american-pathology-partners/security/american-pathology-partners-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pathology
- Laboratory Services
- Healthcare
- Diagnostics
---
