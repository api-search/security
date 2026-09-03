---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unison.com
  spf: true
hosts:
- cert_expires: Nov 22 18:16:35 2026 GMT
  host: www.unison.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unison, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unison
provider_slug: unison
slug: unison-domain-security
source_filename: unison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unison.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 18:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unison.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unison/refs/heads/main/security/unison-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Real Estate
- Home Equity
- Mortgage
- Consumer Finance
- Investment Management
---
