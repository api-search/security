---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ons.gov.uk
  spf: true
hosts:
- cert_expires: Dec  2 06:29:24 2026 GMT
  host: www.ons.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Office For National Statistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office for National Statistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Office for National Statistics
provider_slug: office-for-national-statistics
slug: office-for-national-statistics-domain-security
source_filename: office-for-national-statistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ons.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 06:29:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ons.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-for-national-statistics/refs/heads/main/security/office-for-national-statistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Statistics
- Data
- United Kingdom
- PublicSector
---
