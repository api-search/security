---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: facets.cloud
  spf: true
hosts:
- cert_expires: Sep 19 23:11:10 2026 GMT
  host: www.facets.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Facets
provider_slug: facets
slug: facets-domain-security
source_filename: facets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.facets.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:11:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: facets.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facets/refs/heads/main/security/facets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Infrastructure
- Orchestration
- Platform Engineering
- DevOps
---
