---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ul.com
  spf: true
hosts:
- cert_expires: Sep 16 11:48:10 2026 GMT
  host: www.ul.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: my.ul.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ul Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UL Solutions, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UL Solutions
provider_slug: ul-solutions
slug: ul-solutions-domain-security
source_filename: ul-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: my.ul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ul-solutions/refs/heads/main/security/ul-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Safety Science
- Certification
- Testing
- Compliance
- Standards
- Inspection
---
