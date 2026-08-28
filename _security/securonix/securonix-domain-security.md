---
api_specs:
- filename: securonix-policy-management-api.json
  format: json
  label: Securonix Policy Management API
  slug: securonix-policy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-policy-management-api.json
- filename: securonix-datasource-onboarding-api.json
  format: json
  label: Securonix Datasource Onboarding API
  slug: securonix-datasource-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-datasource-onboarding-api.json
- filename: securonix-device-monitoring-api.json
  format: json
  label: Securonix Device Monitoring API
  slug: securonix-device-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-device-monitoring-api.json
- filename: securonix-threatq-api.json
  format: json
  label: Securonix ThreatQ API
  slug: securonix-threatq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-threatq-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: securonix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: securonix.net
  spf: false
hosts:
- cert_expires: Oct 17 20:32:32 2026 GMT
  host: www.securonix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 01:46:35 2026 GMT
  host: documentation.securonix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: policymanagement.api.securonix.net
  https: false
kind: domain-security
layout: security
method: probed
name: Securonix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securonix, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Securonix
provider_slug: securonix
slug: securonix-domain-security
source_filename: securonix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securonix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 20:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.securonix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: policymanagement.api.securonix.net\n  https: false\ndomains:\n- domain: securonix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: securonix.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/security/securonix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- SIEM
- UEBA
- SOAR
- Threat Intelligence
- Security Analytics
- Cybersecurity
- Log Management
- Detection and Response
- MITRE ATT&CK
---
