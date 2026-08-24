---
api_specs:
- filename: growthspace-public-api-management-openapi-original.yml
  format: yaml
  label: Growthspace Public API Management
  slug: growthspace-public-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-public-api-management-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: growthspace.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appspot.com
  spf: true
hosts:
- cert_expires: Nov 18 16:37:17 2026 GMT
  host: www.growthspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 20:41:53 2026 GMT
  host: public-api-management-dot-growthspace-246311.oa.r.appspot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Growthspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowthSpace, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GrowthSpace
provider_slug: growthspace
slug: growthspace-domain-security
source_filename: growthspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.growthspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 16:37:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api-management-dot-growthspace-246311.oa.r.appspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 20:41:53 2026 GMT\n  hsts: false\ndomains:\n- domain: growthspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: appspot.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/security/growthspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Learning and Development
- Talent Development
- Human Resources
- Coaching
- Employee Experience
- Skills
- Workforce
- Enterprise Software
- Artificial Intelligence
---
