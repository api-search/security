---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oods-foundry.com
  spf: true
hosts:
- cert_expires: Dec 21 19:40:01 2026 GMT
  host: oods-foundry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OODS Foundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OODS Foundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OODS Foundry
provider_slug: oods-foundry-com
slug: oods-foundry-com-domain-security
source_filename: oods-foundry-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oods-foundry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 19:40:01 2026 GMT\n  hsts: false\ndomains:\n- domain: oods-foundry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oods-foundry-com/security/oods-foundry-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Design Systems
- UI
- Open Source
- JavaScript
- React
- Vue
---
