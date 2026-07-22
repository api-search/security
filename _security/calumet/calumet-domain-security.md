---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calumet.com
  spf: true
hosts:
- cert_expires: Aug 22 10:03:53 2026 GMT
  host: calumet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calumet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calumet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calumet
provider_slug: calumet
slug: calumet-domain-security
source_filename: calumet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calumet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calumet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calumet/refs/heads/main/security/calumet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Specialty Chemicals
- Hydrocarbons
- Renewable Fuels
- Lubricants
- Fortune 500
---
