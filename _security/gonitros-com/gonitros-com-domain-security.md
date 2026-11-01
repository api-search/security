---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gonitros.com
  spf: true
hosts:
- cert_expires: Jan 19 17:47:27 2027 GMT
  host: gonitros.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gonitros Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoNitro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoNitro
provider_slug: gonitros-com
slug: gonitros-com-domain-security
source_filename: gonitros-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gonitros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 17:47:27 2027 GMT\n  hsts: false\ndomains:\n- domain: gonitros.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gonitros-com/security/gonitros-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- e-commerce
- Shopify
- DigitalProducts
- API
---
