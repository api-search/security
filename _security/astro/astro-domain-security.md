---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astronauts.id
  spf: true
hosts:
- cert_expires: Sep 18 20:42:59 2026 GMT
  host: www.astronauts.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astro
provider_slug: astro
slug: astro-domain-security
source_filename: astro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astronauts.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:42:59 2026 GMT\n  hsts: false\ndomains:\n- domain: astronauts.id\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astro/refs/heads/main/security/astro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Quick Commerce
- Grocery Delivery
- E-commerce
- Retail
- Indonesia
- On-Demand Delivery
---
