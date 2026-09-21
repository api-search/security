---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capriholdings.com
  spf: true
hosts:
- cert_expires: Nov 30 15:23:41 2026 GMT
  host: www.capriholdings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capri Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capri Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capri Holdings
provider_slug: capri-holdings
slug: capri-holdings-domain-security
source_filename: capri-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capriholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 15:23:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capriholdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capri-holdings/refs/heads/main/security/capri-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Luxury
- Fashion
- Apparel
- Footwear
- Accessories
- Holding Company
- No Developer Program
---
