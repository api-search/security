---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: textron.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: txtav.com
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.textron.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 23:59:59 2026 GMT
  host: txtav.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 13 22:22:41 2026 GMT
  host: www.bellflight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Textron, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Textron
provider_slug: textron
slug: textron-domain-security
source_filename: textron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.textron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: txtav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  6 23:59:59 2026 GMT\n  hsts: false\n- host: www.bellflight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:22:41 2026 GMT\n  hsts: false\ndomains:\n- domain: textron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: txtav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textron/refs/heads/main/security/textron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Aviation
- Defense
- Fortune 500
- Industrial
- Manufacturing
---
