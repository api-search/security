---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goediphi.com
  spf: true
hosts:
- cert_expires: Dec  3 21:14:25 2026 GMT
  host: goediphi.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goediphi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ediphi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ediphi
provider_slug: goediphi-com
slug: goediphi-com-domain-security
source_filename: goediphi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goediphi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 21:14:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: goediphi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goediphi-com/security/goediphi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Education
- VR
- AI
---
