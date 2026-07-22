---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sverve.com
  spf: true
hosts:
- cert_expires: Sep 28 19:45:54 2026 GMT
  host: sverve.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sverve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sverve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sverve
provider_slug: sverve
slug: sverve-domain-security
source_filename: sverve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sverve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:45:54 2026 GMT\n  hsts: null\ndomains:\n- domain: sverve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sverve/refs/heads/main/security/sverve-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Portfolio Lead
- 500 Global
- Inactive
- Influencer Marketing
---
