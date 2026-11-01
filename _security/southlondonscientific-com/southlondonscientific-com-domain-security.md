---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: southlondonscientific.com
  spf: false
hosts:
- cert_expires: Dec 30 04:22:31 2026 GMT
  host: southlondonscientific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Southlondonscientific Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for southlondonscientific-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: southlondonscientific-com
provider_slug: southlondonscientific-com
slug: southlondonscientific-com-domain-security
source_filename: southlondonscientific-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: southlondonscientific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 04:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southlondonscientific.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/southlondonscientific-com/security/southlondonscientific-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Air Quality
- Data
- Consultancy
- Open Source
---
