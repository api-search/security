---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: new.estate
  spf: true
hosts:
- cert_expires: Dec 31 13:55:10 2026 GMT
  host: new.estate
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: New Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New Estate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: New Estate
provider_slug: new-estate
slug: new-estate-domain-security
source_filename: new-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: new.estate\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:55:10 2026 GMT\n  hsts: null\ndomains:\n- domain: new.estate\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/new-estate/security/new-estate-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Real Estate
- Listings
- Platform
- Property
---
