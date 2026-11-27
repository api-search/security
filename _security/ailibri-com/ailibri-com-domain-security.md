---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ailibri.com
  spf: true
hosts:
- cert_expires: Jan 28 03:44:53 2027 GMT
  host: ailibri.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ailibri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ailibri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ailibri
provider_slug: ailibri-com
slug: ailibri-com-domain-security
source_filename: ailibri-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ailibri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 03:44:53 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: ailibri.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ailibri-com/security/ailibri-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Artificial Intelligence
- Catalog
- Russian
- Tools
- Services
---
