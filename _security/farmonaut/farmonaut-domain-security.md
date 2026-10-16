---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: farmonaut.com
  spf: true
hosts:
- cert_expires: Jan  5 18:16:41 2027 GMT
  host: farmonaut.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farmonaut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmonaut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Farmonaut
provider_slug: farmonaut
slug: farmonaut-domain-security
source_filename: farmonaut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmonaut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 18:16:41 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: farmonaut.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmonaut/refs/heads/main/security/farmonaut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
