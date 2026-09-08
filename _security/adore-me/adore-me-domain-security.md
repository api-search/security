---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adoreme.com
  spf: true
hosts:
- cert_expires: Dec  4 03:13:52 2026 GMT
  host: www.adoreme.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adore Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adore Me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adore Me
provider_slug: adore-me
slug: adore-me-domain-security
source_filename: adore-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adoreme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 03:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: adoreme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adore-me/refs/heads/main/security/adore-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Apparel
- Intimate Apparel
- Direct to Consumer
- Fashion
- Consumer
- Subscription Commerce
- Mobile
---
