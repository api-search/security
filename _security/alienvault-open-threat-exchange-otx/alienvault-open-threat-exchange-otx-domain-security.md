---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alienvault.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: otx.alienvault.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alienvault Open Threat Exchange Otx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlienVault Open Threat Exchange (OTX), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AlienVault Open Threat Exchange (OTX)
provider_slug: alienvault-open-threat-exchange-otx
slug: alienvault-open-threat-exchange-otx-domain-security
source_filename: alienvault-open-threat-exchange-otx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otx.alienvault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alienvault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alienvault-open-threat-exchange-otx/refs/heads/main/security/alienvault-open-threat-exchange-otx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anti Malware
- Public APIs
---
