---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rapattoni.com
  spf: true
hosts:
- cert_expires: Mar 11 18:22:09 2027 GMT
  host: rapattoni.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rapattoni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rapattoni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rapattoni
provider_slug: rapattoni
slug: rapattoni-domain-security
source_filename: rapattoni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapattoni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 18:22:09 2027 GMT\n  hsts: null\ndomains:\n- domain: rapattoni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapattoni/refs/heads/main/security/rapattoni-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- MLS
- RESO Web API
- RETS
- Association Management
---
