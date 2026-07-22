---
api_specs:
- filename: phenom-platform-openapi.yml
  format: yaml
  label: Phenom Talent Experience Platform API
  slug: phenom-talent-experience-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: phenom.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: phenompro.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.phenom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: developer.phenom.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api-qa.phenompro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phenom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phenom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Phenom
provider_slug: phenom
slug: phenom-domain-security
source_filename: phenom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phenom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.phenom.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: api-qa.phenompro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phenom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: phenompro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/security/phenom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hr Tech
- Talent Experience
- Recruiting
- Applicant Tracking
- Candidate Experience
- Onboarding
- SCIM
- Resume Parsing
- Skills
- Artificial Intelligence
---
