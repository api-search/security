---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: otwarteapi.pl
  spf: true
hosts:
- cert_expires: Dec 26 02:22:03 2026 GMT
  host: otwarteapi.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otwarteapi Pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for otwarteapi-pl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: otwarteapi-pl
provider_slug: otwarteapi-pl
slug: otwarteapi-pl-domain-security
source_filename: otwarteapi-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otwarteapi.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 02:22:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: otwarteapi.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/otwarteapi-pl/security/otwarteapi-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- OpenData
- Government
- API-Catalog
- Poland
---
