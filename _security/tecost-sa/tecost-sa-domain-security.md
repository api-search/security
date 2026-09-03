---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tecost.ch
  spf: true
hosts:
- cert_expires: Oct 19 08:56:21 2026 GMT
  host: www.tecost.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tecost Sa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tecost SA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tecost SA
provider_slug: tecost-sa
slug: tecost-sa-domain-security
source_filename: tecost-sa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tecost.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 08:56:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tecost.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecost-sa/refs/heads/main/security/tecost-sa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Electronic Health Records
- Clinical Information Systems
- openEHR
- Interoperability
- Hospital Software
- Long-Term Care
- Home Care
- Switzerland
---
