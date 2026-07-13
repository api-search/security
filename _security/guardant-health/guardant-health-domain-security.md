---
api_specs:
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health EMR Ordering Integration
  slug: guardant-health-emr-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health Results Delivery Integration
  slug: guardant-health-results-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guardanthealth.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.guardanthealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: guardanthealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: portal.guardanthealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guardant Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guardant Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Guardant Health
provider_slug: guardant-health
slug: guardant-health-domain-security
source_filename: guardant-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guardanthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: guardanthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: portal.guardanthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: guardanthealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/security/guardant-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Precision Oncology
- Liquid Biopsy
- Genomics
- EMR Integration
---
