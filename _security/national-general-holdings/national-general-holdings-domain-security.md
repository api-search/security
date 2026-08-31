---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nationalgeneral.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.nationalgeneral.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: National General Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National General Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National General Holdings
provider_slug: national-general-holdings
slug: national-general-holdings-domain-security
source_filename: national-general-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nationalgeneral.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nationalgeneral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-general-holdings/refs/heads/main/security/national-general-holdings-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Insurance
- Property & Casualty
- Auto Insurance
- Accident & Health Insurance
- Acquired
- Defunct Standalone
---
