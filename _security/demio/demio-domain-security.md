---
api_specs:
- filename: demio-openapi.yml
  format: yaml
  label: Demio Events API
  slug: demio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-openapi.yml
- filename: demio-openapi.yml
  format: yaml
  label: Demio Reports API
  slug: demio-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-openapi.yml
- filename: demio-openapi.yml
  format: yaml
  label: Demio Intro API
  slug: demio-intro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: demio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Oct  6 17:44:37 2026 GMT
  host: www.demio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: publicdemioapi.docs.apiary.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: my.demio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Demio
provider_slug: demio
slug: demio-domain-security
source_filename: demio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.demio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: publicdemioapi.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\n- host: my.demio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: demio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/security/demio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Webinars
- Virtual Events
- Event Management
- Marketing
- Marketing Technology
- Demand Generation
- Video
- Engagement Marketing
- Lead Generation
- Software-as-a-Service
---
