---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bmi.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: bmi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bmi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BMI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BMI
provider_slug: bmi
slug: bmi-domain-security
source_filename: bmi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bmi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bmi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmi/refs/heads/main/security/bmi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Music
- Royalties
- Licensing
- Advocacy
---
