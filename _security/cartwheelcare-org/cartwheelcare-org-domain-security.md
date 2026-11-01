---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cartwheelcare.org
  spf: true
hosts:
- cert_expires: Dec 12 06:30:03 2026 GMT
  host: cartwheelcare.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cartwheelcare Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartwheel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cartwheel
provider_slug: cartwheelcare-org
slug: cartwheelcare-org-domain-security
source_filename: cartwheelcare-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartwheelcare.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 06:30:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cartwheelcare.org\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cartwheelcare-org/security/cartwheelcare-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- MentalHealth
- Education
- B2B
- SaaS
- Healthcare
---
