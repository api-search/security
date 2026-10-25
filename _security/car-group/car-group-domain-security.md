---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cargroup.com
  spf: true
hosts:
- cert_expires: Jan 12 23:21:58 2027 GMT
  host: cargroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Car Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAR Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CAR Group
provider_slug: car-group
slug: car-group-domain-security
source_filename: car-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cargroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:21:58 2027 GMT\n  hsts: false\ndomains:\n- domain: cargroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/car-group/refs/heads/main/security/car-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Marketplaces
- Classifieds
- Advertising
- Australia
- ASX
---
