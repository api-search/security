---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ellevest.com
  spf: true
hosts:
- cert_expires: Sep 21 02:34:26 2026 GMT
  host: www.ellevest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ellevest.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ellevest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ellevest, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ellevest
provider_slug: ellevest
slug: ellevest-domain-security
source_filename: ellevest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ellevest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:34:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ellevest.com\n  https: false\ndomains:\n- domain: ellevest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellevest/refs/heads/main/security/ellevest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Wealth Management
- Investing
- Financial Planning
- Women Finance
- Robo-Advisory
- Portfolio Management
---
