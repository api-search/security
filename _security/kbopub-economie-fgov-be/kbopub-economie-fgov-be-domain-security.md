---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fgov.be
  spf: true
hosts:
- cert_expires: Mar 15 23:56:37 2027 GMT
  host: kbopub.economie.fgov.be
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crossroads Bank for Enterprises (CBE / KBO / BCE) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossroads Bank for Enterprises (CBE / KBO / BCE), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Crossroads Bank for Enterprises (CBE / KBO / BCE)
provider_slug: kbopub-economie-fgov-be
slug: kbopub-economie-fgov-be-domain-security
source_filename: kbopub-economie-fgov-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kbopub.economie.fgov.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:56:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fgov.be\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kbopub-economie-fgov-be/security/kbopub-economie-fgov-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Belgium
- Business Registry
- Open Data
- Company Data
---
