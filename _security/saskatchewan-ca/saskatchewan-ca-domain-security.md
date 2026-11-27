---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saskatchewan.ca
  spf: true
hosts:
- cert_expires: Jan 16 19:15:01 2027 GMT
  host: gis.saskatchewan.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Government of Saskatchewan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Government of Saskatchewan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Government of Saskatchewan
provider_slug: saskatchewan-ca
slug: saskatchewan-ca-domain-security
source_filename: saskatchewan-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gis.saskatchewan.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 19:15:01 2027 GMT\n  hsts: false\ndomains:\n- domain: saskatchewan.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saskatchewan-ca/security/saskatchewan-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- GIS
- Open Data
- Canada
- Saskatchewan
---
