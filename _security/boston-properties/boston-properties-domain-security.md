---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bxp.com
  spf: true
hosts:
- cert_expires: Aug 21 19:32:52 2026 GMT
  host: www.bxp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boston Properties Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boston Properties (BXP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boston Properties (BXP)
provider_slug: boston-properties
slug: boston-properties-domain-security
source_filename: boston-properties-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bxp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:32:52 2026 GMT\n  hsts: false\ndomains:\n- domain: bxp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boston-properties/refs/heads/main/security/boston-properties-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Commercial Real Estate
- REIT
- Office Properties
- Workplace
- Fortune 1000
---
