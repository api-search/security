---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucidrents.com
  spf: true
hosts:
- cert_expires: Jan 29 00:20:37 2027 GMT
  host: lucidrents.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lucid Rents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucid Rents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucid Rents
provider_slug: lucidrents-com
slug: lucidrents-com-domain-security
source_filename: lucidrents-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucidrents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 00:20:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lucidrents.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lucidrents-com/security/lucidrents-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Data Platform
- NYC
- Transparency
- Rentals
---
