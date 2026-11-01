---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keep.com
  spf: true
hosts:
- cert_expires: Dec 16 02:32:31 2026 GMT
  host: www.keep.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keep Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keep
provider_slug: keep-com
slug: keep-com-domain-security
source_filename: keep-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 02:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: keep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/keep-com/security/keep-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- e-commerce
- retail
- platform
- Shopify
- marketplace
---
