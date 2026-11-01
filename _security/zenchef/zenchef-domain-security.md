---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenchef.com
  spf: true
hosts:
- cert_expires: Jan  8 10:52:11 2027 GMT
  host: zenchef.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zenchef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenchef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zenchef
provider_slug: zenchef
slug: zenchef-domain-security
source_filename: zenchef-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenchef.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:52:11 2027 GMT\n  hsts: false\ndomains:\n- domain: zenchef.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zenchef/security/zenchef-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- SaaS
- Reservations
- Payments
- Analytics
- Company
---
