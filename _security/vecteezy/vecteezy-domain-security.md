---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vecteezy.com
  spf: false
hosts:
- cert_expires: Feb  7 05:38:55 2027 GMT
  host: vecteezy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vecteezy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vecteezy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Vecteezy
provider_slug: vecteezy
slug: vecteezy-domain-security
source_filename: vecteezy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vecteezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 05:38:55 2027 GMT\n  hsts: null\ndomains:\n- domain: vecteezy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/vecteezy/security/vecteezy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
