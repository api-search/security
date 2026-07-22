---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabletics.com
  spf: true
hosts:
- cert_expires: Sep 12 04:18:12 2026 GMT
  host: fabletics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabletics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabletics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fabletics
provider_slug: fabletics
slug: fabletics-domain-security
source_filename: fabletics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabletics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:18:12 2026 GMT\n  hsts: null\ndomains:\n- domain: fabletics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabletics/refs/heads/main/security/fabletics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Apparel
- Athleisure
- Subscription
- Fashion
---
