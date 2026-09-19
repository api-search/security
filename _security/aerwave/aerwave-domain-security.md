---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aerwave.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: getaerwave.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:mailgun.org -all
hosts:
- cert_expires: Nov  7 20:01:08 2026 GMT
  host: www.aerwave.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 13:52:13 2026 GMT
  host: getaerwave.com
  hsts: false
  hsts_max_age: null
  https: true
  note: redirects (HTTP 301) to www.aerwave.com
  tls_version: TLSv1.3
- cert_expires: Oct 26 18:12:48 2026 GMT
  host: portal.getaerwave.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Blazor WebAssembly resident portal (ResidentPortal.Client), Azure-hosted
  tls_version: TLSv1.3
- cert_expires: Oct 26 16:09:56 2026 GMT
  host: register.getaerwave.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Blazor resident registration app, Azure-hosted
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Aerwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerwave, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aerwave
provider_slug: aerwave
slug: aerwave-domain-security
source_filename: aerwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aerwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 20:01:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: getaerwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:52:13 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: redirects (HTTP 301) to www.aerwave.com\n- host: portal.getaerwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 18:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: Blazor WebAssembly resident portal (ResidentPortal.Client), Azure-hosted\n- host: register.getaerwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 16:09:56 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: Blazor resident registration app, Azure-hosted\ndomains:\n- domain: aerwave.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n- domain: getaerwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:mailgun.org -all\n  dmarc: false\n  dmarc_policy: null\nnotes:\n- >-\n  getaerwave.com carries no DMARC record and no CAA record, while aerwave.com\n  publishes DMARC at p=none (monitor only) and also no CAA. Probed 2026-09-12.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerwave/refs/heads/main/security/aerwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Managed WiFi
- Multifamily
- Real-Estate
- Telecommunications
- Internet Service Provider
- Connectivity
- Smart Buildings
- PropTech
---
