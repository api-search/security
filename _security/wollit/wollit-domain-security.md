---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wollit.com
  spf: true
hosts:
- cert_expires: Sep  8 03:32:10 2026 GMT
  host: www.wollit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wollit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wollit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wollit
provider_slug: wollit
slug: wollit-domain-security
source_filename: wollit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wollit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wollit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wollit/refs/heads/main/security/wollit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Credit
- Credit Building
- Personal Finance
- Consumer Finance
- United Kingdom
- Rent Reporting
---
