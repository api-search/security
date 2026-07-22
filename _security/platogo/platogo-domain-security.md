---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: platogo.com
  spf: true
hosts:
- cert_expires: Sep 29 18:33:51 2026 GMT
  host: platogo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Platogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platogo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Platogo
provider_slug: platogo
slug: platogo-domain-security
source_filename: platogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platogo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:33:51 2026 GMT\n  hsts: false\ndomains:\n- domain: platogo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platogo/refs/heads/main/security/platogo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- Social Casino
- Mobile Games
- Casino Games
- Entertainment
- Free-to-Play
---
