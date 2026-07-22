---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grace.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: grace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wr Grace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for W. R. Grace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: W. R. Grace
provider_slug: wr-grace
slug: wr-grace-domain-security
source_filename: wr-grace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grace.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wr-grace/refs/heads/main/security/wr-grace-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Specialty Chemicals
- Catalysts
- Materials Science
- Pharmaceutical
- Refining
- Petrochemicals
---
