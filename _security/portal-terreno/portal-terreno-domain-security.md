---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: portalterreno.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: portalterreno.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portal Terreno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal Terreno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Portal Terreno
provider_slug: portal-terreno
slug: portal-terreno-domain-security
source_filename: portal-terreno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portalterreno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: portalterreno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portal-terreno/refs/heads/main/security/portal-terreno-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Classifieds
- Marketplace
- Land
- Property
- Chile
- Mexico
---
