---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: west.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: westcx.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.west.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 03:02:28 2026 GMT
  host: www.westcx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: West Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for West Technology Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: West Technology Group
provider_slug: west
slug: west-domain-security
source_filename: west-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.west.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: www.westcx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: west.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: westcx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/west/refs/heads/main/security/west-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Experience
- Communications
- Artificial Intelligence
- Healthcare
- Patient Engagement
- Fortune 1000
---
