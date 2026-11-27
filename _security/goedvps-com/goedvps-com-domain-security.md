---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goedvps.com
  spf: true
hosts:
- cert_expires: Feb  4 01:56:37 2027 GMT
  host: goedvps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GoedVPS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoedVPS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoedVPS
provider_slug: goedvps-com
slug: goedvps-com-domain-security
source_filename: goedvps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goedvps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 01:56:37 2027 GMT\n  hsts: false\ndomains:\n- domain: goedvps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/goedvps-com/security/goedvps-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Hosting
- Artificial Intelligence
- GDPR
- Netherlands
---
