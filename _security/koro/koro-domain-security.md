---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: koro.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: korodrogerie.de
  spf: true
hosts:
- cert_expires: Sep 10 23:20:08 2026 GMT
  host: www.koro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:28:27 2026 GMT
  host: www.korodrogerie.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KoRo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: KoRo
provider_slug: koro
slug: koro-domain-security
source_filename: koro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:20:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.korodrogerie.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:28:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: koro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: korodrogerie.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koro/refs/heads/main/security/koro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- E-Commerce
- Food and Beverage
- Retail
- Direct to Consumer
- Germany
- Shopware
- Open Source
---
