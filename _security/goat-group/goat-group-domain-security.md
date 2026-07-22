---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goatgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goat.com
  spf: true
hosts:
- cert_expires: Aug 21 08:32:20 2026 GMT
  host: www.goatgroup.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:38:16 2026 GMT
  host: www.goat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:45:11 2026 GMT
  host: www.grailed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Goat Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goat Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goat Group
provider_slug: goat-group
slug: goat-group-domain-security
source_filename: goat-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goatgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.goat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:38:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.grailed.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 03:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goatgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: goat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goat-group/refs/heads/main/security/goat-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Ecommerce
- Sneakers
- Apparel
- Fashion
- Resale
- Authentication
- Consumer
- Retail
---
