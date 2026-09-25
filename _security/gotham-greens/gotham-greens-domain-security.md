---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gothamgreens.com
  spf: true
hosts:
- cert_expires: Sep 29 13:00:54 2026 GMT
  host: www.gothamgreens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gotham Greens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gotham Greens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Gotham Greens
provider_slug: gotham-greens
slug: gotham-greens-domain-security
source_filename: gotham-greens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gothamgreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:00:54 2026 GMT\n  hsts: false\ndomains:\n- domain: gothamgreens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotham-greens/refs/heads/main/security/gotham-greens-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Agriculture
- Controlled Environment Agriculture
- Hydroponics
- Food
- Consumer Packaged Goods
- Fresh Produce
- Sustainability
- Urban Farming
---
