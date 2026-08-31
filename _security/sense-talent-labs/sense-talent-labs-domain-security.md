---
api_specs:
- filename: sense-talent-labs-appointment-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Appointment API
  slug: sense-talent-labs-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-appointment-api-openapi.yml
- filename: sense-talent-labs-authentication-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Authentication API
  slug: sense-talent-labs-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-authentication-api-openapi.yml
- filename: sense-talent-labs-candidate-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Candidate API
  slug: sense-talent-labs-candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-candidate-api-openapi.yml
- filename: sense-talent-labs-certification-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Certification API
  slug: sense-talent-labs-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-certification-api-openapi.yml
- filename: sense-talent-labs-clientcontact-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Client Contact API
  slug: sense-talent-labs-clientcontact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-clientcontact-api-openapi.yml
- filename: sense-talent-labs-company-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Company API
  slug: sense-talent-labs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-company-api-openapi.yml
- filename: sense-talent-labs-internaluser-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Internal User API
  slug: sense-talent-labs-internaluser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-internaluser-api-openapi.yml
- filename: sense-talent-labs-joborder-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Job Order API
  slug: sense-talent-labs-joborder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-joborder-api-openapi.yml
- filename: sense-talent-labs-lead-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Lead API
  slug: sense-talent-labs-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-lead-api-openapi.yml
- filename: sense-talent-labs-placement-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Placement API
  slug: sense-talent-labs-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-placement-api-openapi.yml
- filename: sense-talent-labs-submission-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Submission API
  slug: sense-talent-labs-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-submission-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sensehq.com
  spf: true
hosts:
- cert_expires: Nov 10 00:56:21 2026 GMT
  host: www.sensehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: developer.sensehq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: partner-api.sensehq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sense Talent Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sense Talent Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sense Talent Labs
provider_slug: sense-talent-labs
slug: sense-talent-labs-domain-security
source_filename: sense-talent-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:56:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sensehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: partner-api.sensehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sensehq.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/security/sense-talent-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Staffing
- Applicant Tracking
- Candidate Engagement
- Recruiting Automation
- Talent CRM
- Messaging
- Interview Scheduling
- Artificial Intelligence
- SaaS
---
