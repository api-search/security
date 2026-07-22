---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uniteddwelling.com
  spf: true
hosts:
- cert_expires: Sep 29 17:29:48 2026 GMT
  host: www.uniteddwelling.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United Dwelling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Dwelling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: United Dwelling
provider_slug: united-dwelling
slug: united-dwelling-domain-security
source_filename: united-dwelling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniteddwelling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:29:48 2026 GMT\n  hsts: null\ndomains:\n- domain: uniteddwelling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-dwelling/refs/heads/main/security/united-dwelling-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Real Estate
- Housing
- Accessory Dwelling Units
- Construction
- Property Management
- Affordable Housing
---
