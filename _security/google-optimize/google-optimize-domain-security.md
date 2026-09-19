---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Nov  2 08:39:48 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:34 2026 GMT
  host: support.google.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:39:03 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Optimize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Optimize, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Optimize
provider_slug: google-optimize
slug: google-optimize-domain-security
source_filename: google-optimize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:39:48 2026 GMT\n  hsts: false\n- host: support.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:34 2026 GMT\n  hsts: null\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:39:03 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-optimize/refs/heads/main/security/google-optimize-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- A/B Testing
- Analytics
- Deprecated
- Experimentation
- Google
- Optimization
- Personalization
- Sunset
---
