---
api_specs:
- filename: levels-health-openapi.yml
  format: yaml
  label: Levels Data Export
  slug: levels-data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levels-health/refs/heads/main/openapi/levels-health-openapi.yml
- filename: levels-health-openapi.yml
  format: yaml
  label: Levels Health Data Integrations
  slug: levels-health-data-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levels-health/refs/heads/main/openapi/levels-health-openapi.yml
- filename: levels-health-openapi.yml
  format: yaml
  label: Levels Partner Program
  slug: levels-partner-program
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levels-health/refs/heads/main/openapi/levels-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: levelshealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: levels.com
  spf: true
hosts:
- cert_expires: Oct  8 17:54:20 2026 GMT
  host: www.levelshealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 00:01:35 2026 GMT
  host: support.levels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levels Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Levels, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Levels
provider_slug: levels-health
slug: levels-health-domain-security
source_filename: levels-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.levelshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:54:20 2026 GMT\n  hsts: false\n- host: support.levels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: levelshealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: levels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levels-health/refs/heads/main/security/levels-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Metabolic Health
- CGM
- Continuous Glucose Monitoring
- Health
- Wellness
---
