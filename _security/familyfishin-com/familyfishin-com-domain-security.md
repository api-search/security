---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: familyfishin.com
  spf: true
hosts:
- cert_expires: Feb  4 20:19:33 2027 GMT
  host: familyfishin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Family Fishin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Family Fishin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Family Fishin
provider_slug: familyfishin-com
slug: familyfishin-com-domain-security
source_filename: familyfishin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: familyfishin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 20:19:33 2027 GMT\n  hsts: false\ndomains:\n- domain: familyfishin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/familyfishin-com/security/familyfishin-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fishing
- Soft-Plastic
- Trout
- Lures
- Missouri
---
