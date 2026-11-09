---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dayze.com
  spf: true
hosts:
- cert_expires: Jan  7 02:47:52 2027 GMT
  host: dayze.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dayze Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dayze-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dayze-com
provider_slug: dayze-com
slug: dayze-com-domain-security
source_filename: dayze-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dayze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 02:47:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dayze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dayze-com/security/dayze-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Context
- Personal CRM
- Life graph
---
