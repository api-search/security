---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laminalabs.ai
  spf: true
hosts:
- cert_expires: Oct  2 18:25:48 2026 GMT
  host: www.laminalabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 10:49:45 2026 GMT
  host: app.laminalabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 21:08:37 2026 GMT
  host: api.laminalabs.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: Recorded from a direct curl HEAD/GET; the mechanical probe returned null because the host answers 401 on every unmatched path.
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lamina Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamina Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lamina Labs
provider_slug: lamina-labs
slug: lamina-labs-domain-security
source_filename: lamina-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laminalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:25:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.laminalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.laminalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: Recorded from a direct curl HEAD/GET; the mechanical probe returned null\n    because the host answers 401 on every unmatched path.\ndomains:\n- domain: laminalabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamina-labs/refs/heads/main/security/lamina-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Machine Learning
- Education
- Media
- Model Context Protocol
- Content Generation
---
