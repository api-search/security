---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentopodata.org
  spf: true
hosts:
- cert_expires: Aug 31 22:51:25 2026 GMT
  host: www.opentopodata.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Topo Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Topo Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open Topo Data
provider_slug: open-topo-data
slug: open-topo-data-domain-security
source_filename: open-topo-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opentopodata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 22:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: opentopodata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-topo-data/refs/heads/main/security/open-topo-data-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Geocoding
- Public APIs
---
