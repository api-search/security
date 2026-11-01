---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ign.es
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.ign.es
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instituto Geogr Fico Nacional Ign Of Spain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instituto Geográfico Nacional (IGN of Spain), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Instituto Geográfico Nacional (IGN of Spain)
provider_slug: instituto-geogr-fico-nacional-ign-of-spain
slug: instituto-geogr-fico-nacional-ign-of-spain-domain-security
source_filename: instituto-geogr-fico-nacional-ign-of-spain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ign.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ign.es\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/instituto-geogr-fico-nacional-ign-of-spain/security/instituto-geogr-fico-nacional-ign-of-spain-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Geospatial
- Government
- Mapping
- Data
- Spain
---
