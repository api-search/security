---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gdynia.pl
  spf: true
hosts:
- cert_expires: Feb 17 12:42:44 2027 GMT
  host: otwartedane.gdynia.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Gdynia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, Gdynia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: City, Gdynia
provider_slug: city-gdynia
slug: city-gdynia-domain-security
source_filename: city-gdynia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otwartedane.gdynia.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 12:42:44 2027 GMT\n  hsts: false\ndomains:\n- domain: gdynia.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-gdynia/refs/heads/main/security/city-gdynia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
