---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: batchgeo.com
  spf: true
hosts:
- cert_expires: Dec 22 13:46:32 2026 GMT
  host: batchgeo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Batchgeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Batchgeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Batchgeo
provider_slug: batchgeo
slug: batchgeo-domain-security
source_filename: batchgeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: batchgeo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 13:46:32 2026 GMT\n  hsts: null\ndomains:\n- domain: batchgeo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/batchgeo/refs/heads/main/security/batchgeo-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Mapping
- Software-as-a-Service
- Data Visualization
- Real Estate
- Sales
---
