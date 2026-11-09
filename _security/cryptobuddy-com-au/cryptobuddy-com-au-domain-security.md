---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cryptobuddy.com.au
  spf: true
hosts:
- cert_expires: Jan 17 21:36:44 2027 GMT
  host: cryptobuddy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cryptobuddy Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cryptobuddy-com-au, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: cryptobuddy-com-au
provider_slug: cryptobuddy-com-au
slug: cryptobuddy-com-au-domain-security
source_filename: cryptobuddy-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptobuddy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:36:44 2027 GMT\n  hsts: null\ndomains:\n- domain: cryptobuddy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cryptobuddy-com-au/security/cryptobuddy-com-au-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
