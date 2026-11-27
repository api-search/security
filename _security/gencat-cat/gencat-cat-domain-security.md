---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transparenciacatalunya.cat
  spf: false
hosts:
- cert_expires: Feb 18 16:08:55 2027 GMT
  host: analisi.transparenciacatalunya.cat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Generalitat de Catalunya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generalitat de Catalunya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Generalitat de Catalunya
provider_slug: gencat-cat
slug: gencat-cat-domain-security
source_filename: gencat-cat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: analisi.transparenciacatalunya.cat\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 16:08:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transparenciacatalunya.cat\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gencat-cat/security/gencat-cat-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Government
- Open Data
- Catalonia
- Transparency
- OData
- Socrata
- Public Sector
---
