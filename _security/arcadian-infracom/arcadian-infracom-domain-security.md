---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcadianinfra.com
  spf: true
hosts:
- cert_expires: Nov  6 02:19:25 2026 GMT
  host: arcadianinfra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcadian Infracom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcadian Infracom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcadian Infracom
provider_slug: arcadian-infracom
slug: arcadian-infracom-domain-security
source_filename: arcadian-infracom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcadianinfra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 02:19:25 2026 GMT\n  hsts: false\ndomains:\n- domain: arcadianinfra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadian-infracom/refs/heads/main/security/arcadian-infracom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Infrastructure
- Fiber
- Broadband
- Rural Connectivity
- St. Louis
---
