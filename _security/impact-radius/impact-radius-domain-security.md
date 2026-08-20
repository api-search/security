---
api_specs:
- filename: impact-radius-brand-account-v14.yml
  format: yaml
  label: impact.com Brand API
  slug: impactcom-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-account-v14.yml
- filename: impact-radius-partner-account-v15.yml
  format: yaml
  label: impact.com Partner API
  slug: impactcom-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-partner-account-v15.yml
- filename: impact-radius-agency-advertisers-v3.yml
  format: yaml
  label: impact.com Agency API
  slug: impactcom-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-agency-advertisers-v3.yml
- filename: impact-radius-brand-advocate-account-v13.yml
  format: yaml
  label: impact.com Advocate API
  slug: impactcom-advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-advocate-account-v13.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: impact.com
  spf: true
hosts:
- cert_expires: Oct  1 22:13:12 2026 GMT
  host: impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 15:33:03 2026 GMT
  host: integrations.impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 18:52:38 2026 GMT
  host: api.impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Impact Radius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impact Radius, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Impact Radius
provider_slug: impact-radius
slug: impact-radius-domain-security
source_filename: impact-radius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:13:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 18:52:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: impact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/security/impact-radius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Partnership Management
- Affiliate Marketing
- Influencer Marketing
- Referral Marketing
- Attribution
- MarTech
- Advocate
- Creator Economy
- E-Commerce
---
