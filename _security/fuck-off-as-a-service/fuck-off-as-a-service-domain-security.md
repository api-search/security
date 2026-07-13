---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foaas.com
  spf: false
hosts:
- cert_expires: Aug 14 15:18:53 2026 GMT
  host: www.foaas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fuck Off As A Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fuck Off as a Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fuck Off as a Service
provider_slug: fuck-off-as-a-service
slug: fuck-off-as-a-service-domain-security
source_filename: fuck-off-as-a-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 15:18:53 2026 GMT\n  hsts: false\ndomains:\n- domain: foaas.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fuck-off-as-a-service/refs/heads/main/security/fuck-off-as-a-service-domain-security.yml
summary_line: TLSv1.3
tags:
- Social
- Public APIs
---
