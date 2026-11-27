---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: civops.io
  spf: true
hosts:
- cert_expires: Dec 27 16:11:51 2026 GMT
  host: civops.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: civops-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for civops-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: civops-io
provider_slug: civops-io
slug: civops-io-domain-security
source_filename: civops-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civops.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: civops.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/civops-io/security/civops-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing Software
- AI Platform
- Operational Analytics
- Contractor Management
---
