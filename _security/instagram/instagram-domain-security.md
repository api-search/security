---
api_specs:
- filename: instagram-graph-api.yaml
  format: yaml
  label: Instagram API with Instagram Login
  slug: instagram-api-with-instagram-login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-graph-api.yaml
- filename: instagram-graph-api.yaml
  format: yaml
  label: Instagram API with Facebook Login
  slug: instagram-api-with-facebook-login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-graph-api.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instagram.com
  spf: true
hosts:
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: graph.instagram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instagram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instagram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instagram
provider_slug: instagram
slug: instagram-domain-security
source_filename: instagram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graph.instagram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instagram.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/security/instagram-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
---
