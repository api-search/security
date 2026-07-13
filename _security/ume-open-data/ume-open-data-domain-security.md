---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: umea.se
  spf: true
hosts:
- cert_expires: Aug 19 10:26:12 2026 GMT
  host: opendata.umea.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ume Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umeå Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Umeå Open Data
provider_slug: ume-open-data
slug: ume-open-data-domain-security
source_filename: ume-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.umea.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:26:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: umea.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ume-open-data/refs/heads/main/security/ume-open-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- Public APIs
---
