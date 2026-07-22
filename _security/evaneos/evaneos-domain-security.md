---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evaneos.com
  spf: true
hosts:
- cert_expires: Aug 25 11:58:34 2026 GMT
  host: www.evaneos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evaneos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evaneos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evaneos
provider_slug: evaneos
slug: evaneos-domain-security
source_filename: evaneos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evaneos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:58:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: evaneos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evaneos/refs/heads/main/security/evaneos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Travel
- Tourism
- Tailor-Made Trips
- Local Agencies
- Sustainable Travel
- B Corp
- France
---
