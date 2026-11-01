---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: secdim.com
  spf: true
hosts:
- cert_expires: Jan 11 06:15:37 2027 GMT
  host: secdim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Secdim Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for secdim-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: secdim-com
provider_slug: secdim-com
slug: secdim-com-domain-security
source_filename: secdim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secdim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 06:15:37 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: secdim.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/secdim-com/security/secdim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Training
- AI
- Developer
---
