---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mysociety.org
  spf: true
hosts:
- cert_expires: Jan 10 06:50:16 2027 GMT
  host: mapit.mysociety.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MapIt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapIt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MapIt
provider_slug: mapit
slug: mapit-domain-security
source_filename: mapit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapit.mysociety.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:50:16 2027 GMT\n  hsts: false\ndomains:\n- domain: mysociety.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mapit/security/mapit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Location
- Mapping
- United Kingdom
- Open Data
---
