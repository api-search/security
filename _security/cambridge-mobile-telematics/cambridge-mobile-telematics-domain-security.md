---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cmtelematics.com
  spf: true
hosts:
- cert_expires: Sep 27 23:13:27 2026 GMT
  host: www.cmtelematics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 12:43:13 2026 GMT
  host: portal.cmtelematics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambridge Mobile Telematics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambridge Mobile Telematics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cambridge Mobile Telematics
provider_slug: cambridge-mobile-telematics
slug: cambridge-mobile-telematics-domain-security
source_filename: cambridge-mobile-telematics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmtelematics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:13:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.cmtelematics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 12:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cmtelematics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambridge-mobile-telematics/refs/heads/main/security/cambridge-mobile-telematics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Telematics
- Insurance
- Mobility
- Usage-Based Insurance
- Fleet Safety
- Connected Vehicle
- SDK
- Crash Detection
---
