---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: collectivemedicaltech.com
  spf: true
hosts:
- cert_expires: Aug 26 04:19:07 2026 GMT
  host: www.collectivemedicaltech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collective Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collective Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Collective Medical
provider_slug: collective-medical
slug: collective-medical-domain-security
source_filename: collective-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.collectivemedicaltech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:19:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: collectivemedicaltech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collective-medical/refs/heads/main/security/collective-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Care Coordination
- Health Information Exchange
- Interoperability
- Population Health
- Care Collaboration
- Acquired
---
