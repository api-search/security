---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: oldtownmedianyc.com
  spf: false
hosts:
- cert_expires: Jan 15 17:37:14 2027 GMT
  host: www.oldtownmedianyc.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oldtownmedianyc Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Old Town Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Old Town Media
provider_slug: oldtownmedianyc-com
slug: oldtownmedianyc-com-domain-security
source_filename: oldtownmedianyc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oldtownmedianyc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 17:37:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: oldtownmedianyc.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/oldtownmedianyc-com/security/oldtownmedianyc-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Media
- Production
- Distribution
- ContentAPI
- NewYork
---
