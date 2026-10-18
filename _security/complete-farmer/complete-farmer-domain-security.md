---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: completefarmer.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: www.completefarmer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Complete Farmer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complete Farmer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Complete Farmer
provider_slug: complete-farmer
slug: complete-farmer-domain-security
source_filename: complete-farmer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.completefarmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: completefarmer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complete-farmer/refs/heads/main/security/complete-farmer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AgTech
- Marketplace
- Africa
- Agriculture
---
