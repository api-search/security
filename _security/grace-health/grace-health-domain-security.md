---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grace.health
  spf: false
hosts:
- cert_expires: Dec 21 07:18:34 2026 GMT
  host: grace.health
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grace Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grace Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Grace Health
provider_slug: grace-health
slug: grace-health-domain-security
source_filename: grace-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grace.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:18:34 2026 GMT\n  hsts: false\ndomains:\n- domain: grace.health\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grace-health/refs/heads/main/security/grace-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
