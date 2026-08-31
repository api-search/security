---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bymiles.co.uk
  note: DMARC is at the strongest policy (p=reject). No CAA records are published and DNSSEC is not enabled on the zone.
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.bymiles.co.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: Marketing site. HSTS max-age is 180 days, below the 1-year preload threshold.
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: api.bymiles.co.uk
  hsts: false
  http_status: 403
  https: true
  note: Private AWS API Gateway serving the By Miles consumer mobile app. Returns 403 ForbiddenException anonymously and emits no Strict-Transport-Security header. Not a public API.
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:48:52 2026 GMT
  host: help.bymiles.co.uk
  hsts: true
  hsts_max_age: 259200
  http_status: 302
  https: true
  note: Zendesk-hosted help centre. HSTS is vendor-set at 3 days, includeSubDomains.
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: docs.bymiles.co.uk
  hsts: false
  http_status: 403
  https: true
  note: AWS CloudFront signed-URL distribution for private policy documents (MissingKey / Key-Pair-Id). Not API documentation.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: By Miles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for By Miles, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: By Miles
provider_slug: by-miles
slug: by-miles-domain-security
source_filename: by-miles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the confirmed-live By Miles subdomains recorded in review.yml\nhosts:\n- host: www.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: Marketing site. HSTS max-age is 180 days, below the 1-year preload threshold.\n- host: api.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n  http_status: 403\n  note: >-\n    Private AWS API Gateway serving the By Miles consumer mobile app. Returns\n    403 ForbiddenException anonymously and emits no Strict-Transport-Security\n    header. Not a public API.\n- host: help.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:48:52 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  http_status: 302\n  note: Zendesk-hosted help centre. HSTS is vendor-set at 3 days, includeSubDomains.\n\
  - host: docs.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n  http_status: 403\n  note: >-\n    AWS CloudFront signed-URL distribution for private policy documents\n    (MissingKey / Key-Pair-Id). Not API documentation.\ndomains:\n- domain: bymiles.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    DMARC is at the strongest policy (p=reject). No CAA records are published\n    and DNSSEC is not enabled on the zone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/by-miles/refs/heads/main/security/by-miles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Motor Insurance
- Usage Based Insurance
- Telematics
- Connected Car
- Direct to Consumer
- Open Banking
- No Public API
---
