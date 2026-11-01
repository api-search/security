---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drayalliance.com
  spf: true
hosts:
- cert_expires: Jan  8 09:07:32 2027 GMT
  host: www.drayalliance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drayalliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drayalliance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drayalliance
provider_slug: drayalliance
slug: drayalliance-domain-security
source_filename: drayalliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drayalliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 09:07:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drayalliance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/drayalliance/security/drayalliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Drayage
- Supply Chain
- API
- Transportation
---
