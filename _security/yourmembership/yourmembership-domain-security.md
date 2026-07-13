---
api_specs:
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Members API
  slug: yourmembership-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Events API
  slug: yourmembership-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Certifications API
  slug: yourmembership-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YMCareers API
  slug: yourmembership-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Content and Community API
  slug: yourmembership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Commerce and Sales API
  slug: yourmembership-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yourmembership.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: careerwebsite.com
  spf: true
hosts:
- cert_expires: Oct  1 19:19:56 2026 GMT
  host: www.yourmembership.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 11:03:41 2026 GMT
  host: ws.yourmembership.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api-doc.careerwebsite.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yourmembership Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YourMembership, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: YourMembership
provider_slug: yourmembership
slug: yourmembership-domain-security
source_filename: yourmembership-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yourmembership.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:19:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ws.yourmembership.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:03:41 2026 GMT\n  hsts: false\n- host: api-doc.careerwebsite.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yourmembership.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: careerwebsite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/security/yourmembership-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- Careers
- Community Brands
- Momentive Software
---
