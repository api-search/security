---
api_specs:
- filename: university-of-north-carolina-at-chapel-hill-dataverse.yaml
  format: yaml
  label: UNC Dataverse API
  slug: dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-north-carolina-at-chapel-hill/refs/heads/main/openapi/university-of-north-carolina-at-chapel-hill-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unc.edu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.org
  spf: true
hosts:
- cert_expires: Aug 23 07:41:31 2026 GMT
  host: www.unc.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: guides.dataverse.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: dataverse.unc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of North Carolina At Chapel Hill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of North Carolina at Chapel Hill, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of North Carolina at Chapel Hill
provider_slug: university-of-north-carolina-at-chapel-hill
slug: university-of-north-carolina-at-chapel-hill-domain-security
source_filename: university-of-north-carolina-at-chapel-hill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:41:31 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: guides.dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\n- host: dataverse.unc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: unc.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dataverse.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-north-carolina-at-chapel-hill/refs/heads/main/security/university-of-north-carolina-at-chapel-hill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Geospatial
- Digital Library
- United States
- North Carolina
---
