---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: karusele.com
  spf: true
hosts:
- cert_expires: Feb  8 07:31:47 2027 GMT
  host: karusele.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Karuselė Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karuselė, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Karuselė
provider_slug: karusele-com
slug: karusele-com-domain-security
source_filename: karusele-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karusele.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 07:31:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: karusele.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/karusele-com/security/karusele-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Manufacturing
- Stainless Steel
- Industrial Components
- B2B
- Lithuania
---
