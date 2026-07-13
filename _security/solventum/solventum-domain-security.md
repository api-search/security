---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solventum.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.solventum.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solventum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solventum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solventum
provider_slug: solventum
slug: solventum-domain-security
source_filename: solventum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solventum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: solventum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solventum/refs/heads/main/security/solventum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- EHR
- Electronic Health Records
- Healthcare
- Healthcare IT
- Health Information Systems
- Medical Devices
- Medical Technology
---
