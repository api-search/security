---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parsyl.com
  spf: true
hosts:
- cert_expires: Nov 18 04:48:14 2026 GMT
  host: www.parsyl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: docs.parsyl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsyl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsyl, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parsyl
provider_slug: parsyl
slug: parsyl-domain-security
source_filename: parsyl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parsyl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 04:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.parsyl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parsyl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsyl/refs/heads/main/security/parsyl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Cargo Insurance
- Supply Chain
- Cold Chain
- Logistics
- Internet of Things
- Sensors
- Risk Management
- Food Safety
- Pharmaceuticals
- Global Health
---
