---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loews.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loewshotels.com
  spf: true
hosts:
- cert_expires: Sep 20 00:28:03 2026 GMT
  host: www.loews.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:27:09 2026 GMT
  host: www.loewshotels.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.cna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loews Corporation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loews Corporation
provider_slug: loews
slug: loews-domain-security
source_filename: loews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:28:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.loewshotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:27:09 2026 GMT\n  hsts: false\n- host: www.cna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: loews.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: loewshotels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loews/refs/heads/main/security/loews-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conglomerate
- Fortune 500
- Holding Company
- Hotels
- Insurance
- Natural Gas
- Packaging
---
