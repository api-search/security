---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adaptive.co
  spf: true
hosts:
- cert_expires: Dec  4 14:53:47 2026 GMT
  host: adaptive.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adaptive Innovations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive Innovations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adaptive Innovations
provider_slug: adaptive-innovations
slug: adaptive-innovations-domain-security
source_filename: adaptive-innovations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adaptive.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 14:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adaptive.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-innovations/refs/heads/main/security/adaptive-innovations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Home Health
- Health Care Services
- Artificial Intelligence
- Clinical Operations
- Medicare
- Care Delivery
---
