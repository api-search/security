---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iconovir.com
  spf: true
hosts:
- cert_expires: Oct  1 09:25:13 2026 GMT
  host: iconovir.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iconovir Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IconOVir Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IconOVir Bio
provider_slug: iconovir-bio
slug: iconovir-bio-domain-security
source_filename: iconovir-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iconovir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:25:13 2026 GMT\n  hsts: false\ndomains:\n- domain: iconovir.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iconovir-bio/refs/heads/main/security/iconovir-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Oncology
- Cancer
- Immunotherapy
- Therapeutics
---
