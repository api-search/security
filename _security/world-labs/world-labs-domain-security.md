---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: worldlabs.ai
  spf: true
hosts:
- cert_expires: Aug 29 20:18:55 2026 GMT
  host: worldlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 15:25:54 2026 GMT
  host: api.worldlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: World Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World Labs
provider_slug: world-labs
slug: world-labs-domain-security
source_filename: world-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worldlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:18:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.worldlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:25:54 2026 GMT\n  hsts: null\ndomains:\n- domain: worldlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-labs/refs/heads/main/security/world-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
---
