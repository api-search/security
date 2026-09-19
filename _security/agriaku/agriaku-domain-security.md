---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agriaku.com
  spf: true
hosts:
- cert_expires: Nov 27 09:19:05 2026 GMT
  host: agriaku.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agriaku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgriAku, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgriAku
provider_slug: agriaku
slug: agriaku-domain-security
source_filename: agriaku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agriaku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 09:19:05 2026 GMT\n  hsts: false\ndomains:\n- domain: agriaku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agriaku/refs/heads/main/security/agriaku-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- AgTech
- E-Commerce
- Marketplace
- Supply Chain
- Distribution
- Indonesia
- B2B
- Mobile
---
