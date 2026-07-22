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
- cert_expires: Sep 21 08:37:24 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:39:19 2026 GMT
  host: monitoring.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:42:48 2026 GMT
  host: logging.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackdriver Google Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stackdriver (Google), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stackdriver (Google)
provider_slug: stackdriver-google
slug: stackdriver-google-domain-security
source_filename: stackdriver-google-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: monitoring.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:39:19 2026 GMT\n  hsts: null\n- host: logging.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:42:48 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackdriver-google/refs/heads/main/security/stackdriver-google-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Infrastructure
- Observability
- Monitoring
- Logging
- Tracing
- Cloud Operations
- Google Cloud
- APIs
---
