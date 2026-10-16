---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcosi.com
  spf: true
hosts:
- cert_expires: Dec 19 07:02:14 2026 GMT
  host: www.getcosi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosihospitality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosihospitality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cosihospitality
provider_slug: cosihospitality
slug: cosihospitality-domain-security
source_filename: cosihospitality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcosi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: getcosi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosihospitality/refs/heads/main/security/cosihospitality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Catering
- FoodTech
- OnlineOrdering
- Hospitality
---
