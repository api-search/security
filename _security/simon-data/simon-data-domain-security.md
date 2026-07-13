---
api_specs:
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
- filename: simon-data-contact-openapi.yml
  format: yaml
  label: Simon Data Contact API
  slug: simon-data-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-contact-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simon.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simondata.com
  spf: true
hosts:
- cert_expires: Oct  2 20:46:55 2026 GMT
  host: www.simon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:24:59 2026 GMT
  host: docs.simondata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: dev.simonsignal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simon Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simon Data, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Simon Data
provider_slug: simon-data
slug: simon-data-domain-security
source_filename: simon-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.simondata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:24:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.simonsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: simon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: simondata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/security/simon-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
---
