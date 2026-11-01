---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gravitymobility.com
  spf: true
hosts:
- cert_expires: Dec 22 13:33:49 2026 GMT
  host: gravitymobility.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gravitymobility Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gravity
provider_slug: gravitymobility-com
slug: gravitymobility-com-domain-security
source_filename: gravitymobility-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gravitymobility.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 13:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gravitymobility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gravitymobility-com/security/gravitymobility-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- EVCharging
- Energy
- Infrastructure
- Mobility
- Technology
---
