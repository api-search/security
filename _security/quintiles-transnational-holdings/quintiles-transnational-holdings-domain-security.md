---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iqvia.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.iqvia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quintiles Transnational Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quintiles Transnational Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quintiles Transnational Holdings
provider_slug: quintiles-transnational-holdings
slug: quintiles-transnational-holdings-domain-security
source_filename: quintiles-transnational-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iqvia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: iqvia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quintiles-transnational-holdings/refs/heads/main/security/quintiles-transnational-holdings-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Pharmaceuticals
- Biotechnology
- Clinical Research
- Healthcare
- Life Sciences
- Fortune 500
---
