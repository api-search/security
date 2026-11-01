---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aonflow.com
  spf: true
hosts:
- cert_expires: Dec  2 21:55:12 2026 GMT
  host: aonflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aonflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAX Software Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DAX Software Solutions
provider_slug: aonflow
slug: aonflow-domain-security
source_filename: aonflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aonflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 21:55:12 2026 GMT\n  hsts: false\ndomains:\n- domain: aonflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aonflow/security/aonflow-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Integration
- iPaaS
- Low-Code
- Automation
---
