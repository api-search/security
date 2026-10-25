---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aristocrat.com
  spf: true
hosts:
- cert_expires: Apr  4 01:41:48 2027 GMT
  host: aristocrat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aristocrat Leisure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aristocrat Leisure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aristocrat Leisure
provider_slug: aristocrat-leisure
slug: aristocrat-leisure-domain-security
source_filename: aristocrat-leisure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aristocrat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 01:41:48 2027 GMT\n  hsts: false\ndomains:\n- domain: aristocrat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aristocrat-leisure/refs/heads/main/security/aristocrat-leisure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Casino Gaming
- Mobile Games
- Gaming Technology
- Entertainment
- Australia
---
