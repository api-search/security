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
- cert_expires: Aug 21 22:58:46 2026 GMT
  host: www.calumet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calumet Specialty Products Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calumet Specialty Products Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calumet Specialty Products Partners
provider_slug: calumet-specialty-products-partners
slug: calumet-specialty-products-partners-domain-security
source_filename: calumet-specialty-products-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.calumet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calumet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calumet-specialty-products-partners/refs/heads/main/security/calumet-specialty-products-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asphalt
- Fuels
- Hydrocarbons
- Lubricants
- Manufacturing
- Petroleum
- Renewable Diesel
- Solvents
- Specialty Chemicals
- Waxes
---
