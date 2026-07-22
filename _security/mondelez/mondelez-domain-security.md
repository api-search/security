---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mondelezinternational.com
  spf: true
hosts:
- cert_expires: Sep 22 00:59:03 2026 GMT
  host: www.mondelezinternational.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mondelez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mondelez, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mondelez
provider_slug: mondelez
slug: mondelez-domain-security
source_filename: mondelez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mondelezinternational.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mondelezinternational.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mondelez/refs/heads/main/security/mondelez-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Food
- Snacks
- Beverages
---
