---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blueowl.com
  spf: true
hosts:
- cert_expires: Sep 22 16:06:44 2026 GMT
  host: www.blueowl.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: developer.blueowl.com
  https: false
- host: api.blueowl.com
  https: false
kind: domain-security
layout: security
method: probed
name: Blue Owl Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Owl Capital, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blue Owl Capital
provider_slug: blue-owl-capital
slug: blue-owl-capital-domain-security
source_filename: blue-owl-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blueowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.blueowl.com\n  https: false\n- host: api.blueowl.com\n  https: false\ndomains:\n- domain: blueowl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-owl-capital/refs/heads/main/security/blue-owl-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alternative Asset Management
- Private Credit
---
