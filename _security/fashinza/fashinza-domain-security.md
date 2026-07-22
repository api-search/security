---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fashinza.com
  spf: false
hosts:
- cert_expires: Sep 10 15:43:44 2026 GMT
  host: fashinza.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fashinza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fashinza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Fashinza
provider_slug: fashinza
slug: fashinza-domain-security
source_filename: fashinza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fashinza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:43:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fashinza.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashinza/refs/heads/main/security/fashinza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Fashion
- Apparel
- Manufacturing
- Supply Chain
- Sourcing
- B2B
---
