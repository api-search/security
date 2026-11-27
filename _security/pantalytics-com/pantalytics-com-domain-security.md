---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pantalytics.com
  spf: true
hosts:
- cert_expires: Jan 16 08:54:37 2027 GMT
  host: pantalytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pantalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantalytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pantalytics
provider_slug: pantalytics-com
slug: pantalytics-com-domain-security
source_filename: pantalytics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pantalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 08:54:37 2027 GMT\n  hsts: false\ndomains:\n- domain: pantalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pantalytics-com/security/pantalytics-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Odoo
- ERP
- Services
---
