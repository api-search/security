---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alaskaair.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.alaskaair.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Alaska Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alaska Airlines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alaska Airlines
provider_slug: alaska-airlines
slug: alaska-airlines-domain-security
source_filename: alaska-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alaskaair.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: alaskaair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alaska-airlines/refs/heads/main/security/alaska-airlines-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Airlines
- Travel
- Transportation
---
