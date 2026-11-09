---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: drafto.eu
  spf: true
hosts:
- cert_expires: Jan 27 22:55:12 2027 GMT
  host: drafto.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drafto Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drafto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Drafto
provider_slug: drafto-eu
slug: drafto-eu-domain-security
source_filename: drafto-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drafto.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 22:55:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: drafto.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/drafto-eu/security/drafto-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Notes
- Productivity
- Sync
- Privacy
---
