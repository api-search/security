---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mapmyindia.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.mapmyindia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mapmyindia Mappls C E Info Systems Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapmyIndia Mappls (C.E. Info Systems Ltd.), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MapmyIndia Mappls (C.E. Info Systems Ltd.)
provider_slug: mapmyindia-mappls-c-e-info-systems-ltd
slug: mapmyindia-mappls-c-e-info-systems-ltd-domain-security
source_filename: mapmyindia-mappls-c-e-info-systems-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mapmyindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mapmyindia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mapmyindia-mappls-c-e-info-systems-ltd/security/mapmyindia-mappls-c-e-info-systems-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mapping
- Location-Intelligence
- IoT
- APIs
- Enterprise
---
