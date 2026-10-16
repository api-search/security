---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carawayhome.com
  spf: true
hosts:
- cert_expires: Dec 14 00:07:32 2026 GMT
  host: www.carawayhome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caraway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caraway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caraway
provider_slug: caraway
slug: caraway-domain-security
source_filename: caraway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carawayhome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 00:07:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carawayhome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caraway/refs/heads/main/security/caraway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cookware
- Sustainable
- HomeGoods
- ECommerce
---
