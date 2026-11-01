---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wearepatchworks.com
  spf: true
hosts:
- cert_expires: Dec 12 12:19:17 2026 GMT
  host: wearepatchworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wearepatchworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patchworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Patchworks
provider_slug: wearepatchworks
slug: wearepatchworks-domain-security
source_filename: wearepatchworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wearepatchworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 12:19:17 2026 GMT\n  hsts: false\ndomains:\n- domain: wearepatchworks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wearepatchworks/security/wearepatchworks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Integration
- eCommerce
- ERP
- Automation
- AI
---
