---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gdprrepresentative.com
  spf: true
hosts:
- cert_expires: Dec 28 07:43:59 2026 GMT
  host: gdprrepresentative.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Europe Services, SE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Europe Services, SE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Europe Services, SE
provider_slug: gdprrepresentative-com
slug: gdprrepresentative-com-domain-security
source_filename: gdprrepresentative-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gdprrepresentative.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 07:43:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gdprrepresentative.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gdprrepresentative-com/security/gdprrepresentative-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- GDPR
- EU-Representative
- Data Protection
- Compliance
- Services
---
