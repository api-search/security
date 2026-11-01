---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Dec  6 13:36:03 2026 GMT
  host: www.eusc.europa.eu
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: European Union Satellite Centre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for European Union Satellite Centre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: European Union Satellite Centre
provider_slug: european-union-satellite-centre
slug: european-union-satellite-centre-domain-security
source_filename: european-union-satellite-centre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eusc.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 13:36:03 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/european-union-satellite-centre/security/european-union-satellite-centre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
