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
kind: domain-security
layout: security
method: probed
name: Fmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FMC Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FMC Corporation
provider_slug: fmc
slug: fmc-domain-security
source_filename: fmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fmc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 22:47:12 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: fmc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fmc/refs/heads/main/security/fmc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agriculture
- Agrochemicals
- Crop Protection
- Industrial
- Fortune 1000
---
