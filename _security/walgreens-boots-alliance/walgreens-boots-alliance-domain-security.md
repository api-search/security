---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: walgreensbootsalliance.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walgreens.com
  spf: true
hosts:
- cert_expires: Aug 30 22:13:25 2026 GMT
  host: www.walgreensbootsalliance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: developer.walgreens.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- host: api.wba.com
  https: false
kind: domain-security
layout: security
method: probed
name: Walgreens Boots Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walgreens Boots Alliance, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Walgreens Boots Alliance
provider_slug: walgreens-boots-alliance
slug: walgreens-boots-alliance-domain-security
source_filename: walgreens-boots-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walgreensbootsalliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 22:13:25 2026 GMT\n  hsts: false\n- host: developer.walgreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.wba.com\n  https: false\ndomains:\n- domain: walgreensbootsalliance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: walgreens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walgreens-boots-alliance/refs/heads/main/security/walgreens-boots-alliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmacy
- Healthcare
- Health Wellbeing
- Retail
- Specialty Pharmacy
- Population Health
---
