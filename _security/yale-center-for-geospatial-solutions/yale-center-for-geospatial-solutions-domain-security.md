---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yale.edu
  spf: true
hosts:
- cert_expires: Jan 14 20:02:45 2027 GMT
  host: geospatial.yale.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yale Center For Geospatial Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yale Center for Geospatial Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yale Center for Geospatial Solutions
provider_slug: yale-center-for-geospatial-solutions
slug: yale-center-for-geospatial-solutions-domain-security
source_filename: yale-center-for-geospatial-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geospatial.yale.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:02:45 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: yale.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/yale-center-for-geospatial-solutions/security/yale-center-for-geospatial-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geospatial
- Research
- Education
- Data
- Yale
---
