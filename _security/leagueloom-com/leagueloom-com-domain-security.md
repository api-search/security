---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: leagueloom.com
  spf: true
hosts:
- cert_expires: Jan 28 07:09:34 2027 GMT
  host: leagueloom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: League Loom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for League Loom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: League Loom
provider_slug: leagueloom-com
slug: leagueloom-com-domain-security
source_filename: leagueloom-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leagueloom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 07:09:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: leagueloom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/leagueloom-com/security/leagueloom-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Fantasy Sports
- Connector
- Free
---
