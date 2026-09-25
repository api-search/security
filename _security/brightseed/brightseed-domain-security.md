---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightseedbio.com
  spf: true
hosts:
- cert_expires: Oct 20 16:36:53 2026 GMT
  host: www.brightseedbio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brightseed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightseed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brightseed
provider_slug: brightseed
slug: brightseed-domain-security
source_filename: brightseed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightseedbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 16:36:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brightseedbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightseed/refs/heads/main/security/brightseed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bioactives
- Artificial Intelligence
- Life Sciences
- Nutrition
- Ingredients
- Drug Discovery
- Agrifood
- content-api
- WordPress
---
