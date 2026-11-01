---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openlegacy.com
  spf: true
hosts:
- cert_expires: Jan 10 12:05:35 2027 GMT
  host: openlegacy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openlegacy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLegacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenLegacy
provider_slug: openlegacy-com
slug: openlegacy-com-domain-security
source_filename: openlegacy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openlegacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:05:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openlegacy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openlegacy-com/security/openlegacy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legacy Modernization
- API Generation
- Low-Code
- Cloud Integration
---
