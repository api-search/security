---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cleanairdata.org
  spf: false
hosts:
- cert_expires: Jan  6 18:11:40 2027 GMT
  host: cleanairdata.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clean Air Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clean Air Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Clean Air Data
provider_slug: cleanairdata-org
slug: cleanairdata-org-domain-security
source_filename: cleanairdata-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleanairdata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:11:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cleanairdata.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cleanairdata-org/security/cleanairdata-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Air Quality
- Data
- EPA
- US Cities
- Rankings
---
