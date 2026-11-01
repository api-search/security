---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esriuk.com
  spf: true
hosts:
- cert_expires: Dec  2 18:12:27 2026 GMT
  host: www.esriuk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Esri Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esri UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Esri UK
provider_slug: esri-uk
slug: esri-uk-domain-security
source_filename: esri-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esriuk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 18:12:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esriuk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/esri-uk/security/esri-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GIS
- Mapping
- Spatial-Analytics
- Enterprise-Software
- UK
---
