---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ki-radar24.de
  spf: true
hosts:
- cert_expires: Jan 27 05:09:38 2027 GMT
  host: ki-radar24.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KIRadar24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KIRadar24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KIRadar24
provider_slug: ki-radar24-de
slug: ki-radar24-de-domain-security
source_filename: ki-radar24-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ki-radar24.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 05:09:38 2027 GMT\n  hsts: false\ndomains:\n- domain: ki-radar24.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ki-radar24-de/security/ki-radar24-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Directory
- Marketplace
- German
- Platform
---
