---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hilltop-holdings.com
  spf: true
hosts:
- cert_expires: Aug 24 18:53:06 2026 GMT
  host: www.hilltop-holdings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.hilltop-holdings.com
  https: false
- host: api.hilltop-holdings.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hilltop Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilltop Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hilltop Holdings
provider_slug: hilltop-holdings
slug: hilltop-holdings-domain-security
source_filename: hilltop-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hilltop-holdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hilltop-holdings.com\n  https: false\n- host: api.hilltop-holdings.com\n  https: false\ndomains:\n- domain: hilltop-holdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilltop-holdings/refs/heads/main/security/hilltop-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Insurance
- Financial Services
---
