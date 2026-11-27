---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hefes.net
  spf: true
hosts:
- cert_expires: Jan 26 23:35:34 2027 GMT
  host: hefes.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hefes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hefes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hefes
provider_slug: hefes-net
slug: hefes-net-domain-security
source_filename: hefes-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hefes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:35:34 2027 GMT\n  hsts: false\ndomains:\n- domain: hefes.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hefes-net/security/hefes-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Software Engineering
- Managed Cloud
- Cryptocurrency
- Infrastructure
- Product
---
