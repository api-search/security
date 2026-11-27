---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tendergap.com
  spf: true
hosts:
- cert_expires: Jan 28 16:34:47 2027 GMT
  host: tendergap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tendergap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tendergap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tendergap
provider_slug: tendergap-com
slug: tendergap-com-domain-security
source_filename: tendergap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tendergap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:34:47 2027 GMT\n  hsts: null\ndomains:\n- domain: tendergap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tendergap-com/security/tendergap-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Market-Intelligence
- API
- Data
- Competitive-Analysis
---
