---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ceresti.com
  spf: true
hosts:
- cert_expires: Nov 28 11:11:04 2026 GMT
  host: www.ceresti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ceresti Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceresti Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ceresti Health
provider_slug: ceresti-health
slug: ceresti-health-domain-security
source_filename: ceresti-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ceresti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 11:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ceresti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceresti-health/refs/heads/main/security/ceresti-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Dementia
- CaregiverSupport
- Health Tech
---
