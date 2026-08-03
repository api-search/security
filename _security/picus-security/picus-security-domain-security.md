---
api_specs:
- filename: picus-security-activity-logs-openapi.yml
  format: yaml
  label: Picus Customer API
  slug: picus-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-activity-logs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: picussecurity.com
  spf: true
hosts:
- cert_expires: Sep 30 13:19:38 2026 GMT
  host: www.picussecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:55:39 2026 GMT
  host: apidocs.picussecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.picussecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picus Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picus Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Picus Security
provider_slug: picus-security
slug: picus-security-domain-security
source_filename: picus-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picussecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:19:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.picussecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:55:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.picussecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: picussecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/security/picus-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- cybersecurity
- security-validation
- breach-and-attack-simulation
- adversarial-exposure-validation
- continuous-threat-exposure-management
- penetration-testing
- threat-intelligence
- mitre-attack
- detection-engineering
- security-operations
---
