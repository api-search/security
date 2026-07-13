---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fmc.com
  spf: true
hosts:
- cert_expires: Jul 25 22:47:12 2026 GMT
  host: www.fmc.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 25 22:11:51 2026 GMT
  host: ag.fmc.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fmc Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FMC Corporation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FMC Corporation
provider_slug: fmc-corporation
slug: fmc-corporation-domain-security
source_filename: fmc-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fmc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 22:47:12 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: ag.fmc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 22:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: fmc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fmc-corporation/refs/heads/main/security/fmc-corporation-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agriculture
- Agricultural Sciences
- Crop Protection
- Plant Health
- Insecticides
- Herbicides
- Fungicides
- Biologicals
- Pheromones
- Precision Agriculture
- Fortune 1000
---
