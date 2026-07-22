---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yourpremierlab.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: safemedicaldata.com
  spf: false
hosts:
- cert_expires: Sep  4 23:44:25 2026 GMT
  host: yourpremierlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 13:06:50 2026 GMT
  host: premierv2.safemedicaldata.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Premier Laboratory Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Premier Laboratory Services, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Premier Laboratory Services
provider_slug: premier-laboratory-services
slug: premier-laboratory-services-domain-security
source_filename: premier-laboratory-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yourpremierlab.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  4 23:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: premierv2.safemedicaldata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 13:06:50 2026 GMT\n  hsts: false\ndomains:\n- domain: yourpremierlab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: safemedicaldata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-laboratory-services/refs/heads/main/security/premier-laboratory-services-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Clinical Laboratory
- Diagnostics
- Healthcare
- Medical Testing
- Louisiana
---
