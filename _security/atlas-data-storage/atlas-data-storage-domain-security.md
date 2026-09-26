---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atlasbase.com
  spf: true
hosts:
- cert_expires: Nov 27 23:56:00 2026 GMT
  host: www.atlasbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlas Data Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas Data Storage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atlas Data Storage
provider_slug: atlas-data-storage
slug: atlas-data-storage-domain-security
source_filename: atlas-data-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atlasbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atlasbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas-data-storage/refs/heads/main/security/atlas-data-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud
- Storage
- Enterprise
- API
- Data Management
---
