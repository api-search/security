---
api_specs:
- filename: employ-inc-status-api-openapi.yml
  format: yaml
  label: Employ Inc Status API
  slug: employ-inc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employ-inc/refs/heads/main/openapi/employ-inc-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: employinc.com
  spf: true
hosts:
- cert_expires: Oct 30 12:26:19 2026 GMT
  host: www.employinc.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 13:23:06 2026 GMT
  host: status.employinc.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Employ Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Employ, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Employ
provider_slug: employ-inc
slug: employ-inc-domain-security
source_filename: employ-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.employinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 12:26:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: status.employinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:23:06 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: employinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employ-inc/refs/heads/main/security/employ-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Applicant Tracking
- Hiring
- Content
- Event
- Status
---
