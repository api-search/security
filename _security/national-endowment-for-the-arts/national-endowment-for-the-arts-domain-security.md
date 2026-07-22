---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arts.gov
  spf: true
hosts:
- cert_expires: Dec  6 01:31:52 2026 GMT
  host: www.arts.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Endowment For The Arts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Endowment for the Arts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Endowment for the Arts
provider_slug: national-endowment-for-the-arts
slug: national-endowment-for-the-arts-domain-security
source_filename: national-endowment-for-the-arts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 01:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arts.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-endowment-for-the-arts/refs/heads/main/security/national-endowment-for-the-arts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Arts
- Federal Government
- Culture
- Grants
---
