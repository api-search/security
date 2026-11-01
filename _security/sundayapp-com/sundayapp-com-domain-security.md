---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sundayapp.com
  spf: true
hosts:
- cert_expires: Jan 13 00:30:05 2027 GMT
  host: www.sundayapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sundayapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sunday
provider_slug: sundayapp-com
slug: sundayapp-com-domain-security
source_filename: sundayapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sundayapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 00:30:05 2027 GMT\n  hsts: null\ndomains:\n- domain: sundayapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sundayapp-com/security/sundayapp-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
