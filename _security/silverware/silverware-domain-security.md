---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silverwarepos.com
  spf: true
hosts:
- cert_expires: Nov 29 11:06:55 2026 GMT
  host: silverwarepos.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Silverware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silverware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Silverware
provider_slug: silverware
slug: silverware-domain-security
source_filename: silverware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silverwarepos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 11:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: silverwarepos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/silverware/security/silverware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- POS
- Restaurants
- Hotels
- Software
---
