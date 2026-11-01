---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 52north.org
  spf: true
hosts:
- cert_expires: Dec 21 22:27:52 2026 GMT
  host: www.52north.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 52 North Spatial Information Research Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 52°North Spatial Information Research GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 52°North Spatial Information Research GmbH
provider_slug: 52-north-spatial-information-research-gmbh
slug: 52-north-spatial-information-research-gmbh-domain-security
source_filename: 52-north-spatial-information-research-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.52north.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 22:27:52 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: 52north.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/52-north-spatial-information-research-gmbh/security/52-north-spatial-information-research-gmbh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geospatial
- Research
- Open-Standards
- Data-Processing
---
