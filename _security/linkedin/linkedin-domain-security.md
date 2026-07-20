---
api_specs:
- filename: overview
  format: yaml
  label: LinkedIn Consumer API
  slug: linkedin-consumer-api
  spec_type: Postman
  url: https://www.postman.com/linkedin-developer-apis/workspace/linkedin-consumer-solutions/overview
- filename: linkedin-marketing-audience-insights.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: linkedin-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-marketing-audience-insights.yml
- filename: linkedin-learning-activity-reports.yml
  format: yaml
  label: LinkedIn Learning Solutions
  slug: linkedin-learning-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-learning-activity-reports.yml
- filename: linkedin-talent-job-posting.yml
  format: yaml
  label: LinkedIn Talent Solutions
  slug: linkedin-talent-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-talent-job-posting.yml
- filename: linkedin-compliance-events.yml
  format: yaml
  label: LinkedIn Compliance Solutions
  slug: linkedin-compliance-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-compliance-events.yml
- filename: linkedin-sales-navigator.yml
  format: yaml
  label: LinkedIn Sales Navigator API
  slug: linkedin-sales-navigator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-sales-navigator.yml
- filename: linkedin-regulations-data-portability.yml
  format: yaml
  label: LinkedIn Regulatory API
  slug: linkedin-regulatory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-regulations-data-portability.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkedin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkedIn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LinkedIn
provider_slug: linkedin
slug: linkedin-domain-security
source_filename: linkedin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/security/linkedin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
- Fortune 1000
---
