---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acnestudios.com
  spf: true
hosts:
- cert_expires: Jan 10 12:26:34 2027 GMT
  host: acnestudios.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acne Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acne Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acne Studios
provider_slug: acne-studios
slug: acne-studios-domain-security
source_filename: acne-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acnestudios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:26:34 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: acnestudios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acne-studios/refs/heads/main/security/acne-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fashion
- Retail
- Apparel
- Ecommerce
- Sweden
---
