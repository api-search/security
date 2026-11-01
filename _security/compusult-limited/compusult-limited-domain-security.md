---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compusult.net
  spf: true
hosts:
- cert_expires: Feb 28 11:53:42 2027 GMT
  host: www.compusult.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compusult Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compusult Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Compusult Limited
provider_slug: compusult-limited
slug: compusult-limited-domain-security
source_filename: compusult-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compusult.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 11:53:42 2027 GMT\n  hsts: false\ndomains:\n- domain: compusult.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/compusult-limited/security/compusult-limited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- Assistive Technology
- Asset Tracking
- Robotics
- Enterprise Software
---
