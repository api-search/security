---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: igo.com.au
  spf: true
hosts:
- cert_expires: Jan  2 05:48:31 2027 GMT
  host: igo.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Igo Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IGO Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IGO Limited
provider_slug: igo-com-au
slug: igo-com-au-domain-security
source_filename: igo-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igo.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:48:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: igo.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igo-com-au/refs/heads/main/security/igo-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Critical Minerals
- Lithium
- Nickel
- Clean Energy
- Australia
---
