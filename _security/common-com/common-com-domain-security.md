---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: common.com
  spf: false
hosts:
- cert_expires: Feb 11 17:11:01 2027 GMT
  host: common.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Common Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Common
provider_slug: common-com
slug: common-com-domain-security
source_filename: common-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: common.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 17:11:01 2027 GMT\n  hsts: null\ndomains:\n- domain: common.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/common-com/security/common-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Integration
- API-Gateway
- Enterprise
- Platform
---
