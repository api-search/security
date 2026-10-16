---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: correos.es
  spf: true
hosts:
- cert_expires: Apr 28 23:59:59 2027 GMT
  host: www.correos.es
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Correos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Correos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Correos
provider_slug: correos
slug: correos-domain-security
source_filename: correos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.correos.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: correos.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/correos/refs/heads/main/security/correos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Postal
- Logistics
- API
- Spain
---
