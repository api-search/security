---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: husqvarnagroup.com
  spf: true
hosts:
- cert_expires: Nov 24 10:36:39 2026 GMT
  host: husqvarnagroup.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Husqvarna Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Husqvarna Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Husqvarna Group
provider_slug: husqvarna-group
slug: husqvarna-group-domain-security
source_filename: husqvarna-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: husqvarnagroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 10:36:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: husqvarnagroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/husqvarna-group/refs/heads/main/security/husqvarna-group-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Outdoor
- PowerTools
- Forestry
- Sustainability
---
