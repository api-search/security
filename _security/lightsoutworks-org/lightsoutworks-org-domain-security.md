---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lightsoutworks.org
  spf: false
hosts:
- cert_expires: Dec 21 17:49:32 2026 GMT
  host: lightsoutworks.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lights Out Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lights Out Works, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lights Out Works
provider_slug: lightsoutworks-org
slug: lightsoutworks-org-domain-security
source_filename: lightsoutworks-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightsoutworks.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 17:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightsoutworks.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lightsoutworks-org/security/lightsoutworks-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Search
- Capabilities
- OpenAPI
- No Auth
- Agents
---
