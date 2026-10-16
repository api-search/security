---
api_specs:
- filename: clinicalauditai-audits-api-openapi.yml
  format: yaml
  label: ClinicalAuditAI Audits API
  slug: clinicalauditai-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinicalauditai/refs/heads/main/openapi/clinicalauditai-audits-api-openapi.yml
- filename: clinicalauditai-client-settings-api-openapi.yml
  format: yaml
  label: ClinicalAuditAI Client Settings API
  slug: clinicalauditai-client-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinicalauditai/refs/heads/main/openapi/clinicalauditai-client-settings-api-openapi.yml
- filename: clinicalauditai-health-api-openapi.yml
  format: yaml
  label: ClinicalAuditAI Health API
  slug: clinicalauditai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinicalauditai/refs/heads/main/openapi/clinicalauditai-health-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clinicalauditai.com
  spf: true
hosts:
- cert_expires: Nov 18 22:48:40 2026 GMT
  host: www.clinicalauditai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clinicalauditai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClinicalAuditAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClinicalAuditAI
provider_slug: clinicalauditai
slug: clinicalauditai-domain-security
source_filename: clinicalauditai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clinicalauditai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 22:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clinicalauditai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clinicalauditai/refs/heads/main/security/clinicalauditai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Clinical Audits
- API
- Automation
---
