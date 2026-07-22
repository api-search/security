---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: joshwoodcolour.com
  spf: true
hosts:
- cert_expires: Sep 27 19:24:42 2026 GMT
  host: joshwoodcolour.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Josh Wood Colour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Josh Wood Colour, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Josh Wood Colour
provider_slug: josh-wood-colour
slug: josh-wood-colour-domain-security
source_filename: josh-wood-colour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joshwoodcolour.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: joshwoodcolour.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/josh-wood-colour/refs/heads/main/security/josh-wood-colour-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- E-Commerce
- Hair Colour
- Beauty
- Consumer Goods
- Shopify
- Direct-to-Consumer
---
