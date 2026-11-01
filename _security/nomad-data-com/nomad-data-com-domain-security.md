---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nomad-data.com
  spf: true
hosts:
- cert_expires: Dec  1 22:32:05 2026 GMT
  host: www.nomad-data.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomad Data Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nomad
provider_slug: nomad-data-com
slug: nomad-data-com-domain-security
source_filename: nomad-data-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nomad-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 22:32:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nomad-data.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nomad-data-com/security/nomad-data-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Catalog
- Document Insights
- Data Relationship Manager
- AI Search
- Data Spend Management
---
