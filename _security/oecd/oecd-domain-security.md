---
api_specs:
- filename: oecd-openapi.yml
  format: yaml
  label: OECD Data API
  slug: oecd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oecd/refs/heads/main/openapi/oecd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oecd.org
  spf: true
hosts:
- cert_expires: Aug 25 05:15:09 2026 GMT
  host: www.oecd.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 05:15:09 2026 GMT
  host: sdmx.oecd.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oecd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OECD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OECD
provider_slug: oecd
slug: oecd-domain-security
source_filename: oecd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oecd.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:15:09 2026 GMT\n  hsts: null\n- host: sdmx.oecd.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:15:09 2026 GMT\n  hsts: null\ndomains:\n- domain: oecd.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oecd/refs/heads/main/security/oecd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Statistics
- Economics
- SDMX
---
