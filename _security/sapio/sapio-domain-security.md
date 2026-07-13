---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sapiosciences.com
  spf: true
hosts:
- cert_expires: Sep 28 10:04:50 2026 GMT
  host: www.sapiosciences.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-instance.sapiosciences.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sapio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapio Sciences, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sapio Sciences
provider_slug: sapio
slug: sapio-domain-security
source_filename: sapio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sapiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-instance.sapiosciences.com\n  https: false\ndomains:\n- domain: sapiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapio/refs/heads/main/security/sapio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LIMS
- ELN
- Laboratory Informatics
- Life Sciences
- Scientific Data
- Lab Automation
- Instrument Integration
- Biotech
- Pharma
---
