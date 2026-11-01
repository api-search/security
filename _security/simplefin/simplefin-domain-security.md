---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplefin.org
  spf: true
hosts:
- cert_expires: Nov 30 15:13:41 2026 GMT
  host: www.simplefin.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simplefin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleFIN Bridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SimpleFIN Bridge
provider_slug: simplefin
slug: simplefin-domain-security
source_filename: simplefin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplefin.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 15:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: simplefin.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/simplefin/security/simplefin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- API
- Open-Source
- Data
---
