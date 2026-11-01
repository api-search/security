---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: airpim.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: airpim.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airpim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openbridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Openbridge
provider_slug: airpim
slug: airpim-domain-security
source_filename: airpim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airpim.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: airpim.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/airpim/security/airpim-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Data Integration
- Automation
- Analytics
- Modular Software
- Openbridge
---
