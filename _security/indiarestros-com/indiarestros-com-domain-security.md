---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: indiarestros.com
  spf: true
hosts:
- cert_expires: Jan  7 04:01:25 2027 GMT
  host: indiarestros.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: indiarestros-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for indiarestros-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: indiarestros-com
provider_slug: indiarestros-com
slug: indiarestros-com-domain-security
source_filename: indiarestros-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indiarestros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 04:01:25 2027 GMT\n  hsts: null\ndomains:\n- domain: indiarestros.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/indiarestros-com/security/indiarestros-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
