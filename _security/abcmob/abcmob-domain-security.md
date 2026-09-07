---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abcmob.com
  spf: true
hosts:
- cert_expires: Oct 28 18:36:02 2026 GMT
  host: abcmob.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abcmob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for abcMob, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: abcMob
provider_slug: abcmob
slug: abcmob-domain-security
source_filename: abcmob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcmob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 18:36:02 2026 GMT\n  hsts: false\ndomains:\n- domain: abcmob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcmob/refs/heads/main/security/abcmob-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mobile
- Mobile Applications
- Application Development
- Enterprise Software
- Cross Platform
- Banking
- Hospitality
- United States
---
