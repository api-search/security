---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mindflows.us
  spf: true
hosts:
- cert_expires: Apr 30 04:55:47 2027 GMT
  host: mindflows.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mindflows Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mindflows-us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mindflows-us
provider_slug: mindflows-us
slug: mindflows-us-domain-security
source_filename: mindflows-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindflows.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 04:55:47 2027 GMT\n  hsts: false\ndomains:\n- domain: mindflows.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mindflows-us/security/mindflows-us-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Knowledge Management
- Visual Workflow
- AI Search
---
