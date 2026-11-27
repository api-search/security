---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: knowngood.sh
  spf: true
hosts:
- cert_expires: Jan 20 02:09:30 2027 GMT
  host: knowngood.sh
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Known Good Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Known Good, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Known Good
provider_slug: knowngood-sh
slug: knowngood-sh-domain-security
source_filename: knowngood-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knowngood.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 02:09:30 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: knowngood.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/knowngood-sh/security/knowngood-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Artificial Intelligence
- Index
- Web
- Open Source
---
