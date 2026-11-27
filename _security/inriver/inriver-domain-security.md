---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inriver.com
  spf: true
hosts:
- cert_expires: Jan 31 00:09:15 2027 GMT
  host: inriver.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inriver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inriver, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inriver
provider_slug: inriver
slug: inriver-domain-security
source_filename: inriver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:09:15 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: inriver.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/inriver/security/inriver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Information Management
- Artificial Intelligence
- Omnichannel
- B2B
---
