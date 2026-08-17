---
api_specs:
- filename: zoca-platform-openapi.yml
  format: yaml
  label: Zoca Platform API
  slug: zoca-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-platform-openapi.yml
- filename: zoca-tasks-openapi.yml
  format: yaml
  label: Zoca Tasks API
  slug: zoca-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-tasks-openapi.yml
- filename: zoca-public-openapi.yml
  format: yaml
  label: Zoca Public API
  slug: zoca-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-public-openapi.yml
certifications:
- HIPAA
description: ''
kind: trust-center
layout: security
name: Zoca Trust Center
name_suffix: Trust Center
overview: Zoca maintains a public trust center documenting HIPAA compliance.
provider_name: Zoca
provider_slug: zoca
slug: zoca-trust-center
source_filename: zoca-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.zoca.com/\nurl: https://trust.zoca.com/\nplatform: Sprinto\nnote: Zoca runs a Sprinto-hosted trust centre at trust.zoca.com. It is served behind CloudFront and returns HTTP\n  403 to a default curl User-Agent; it renders normally with a browser User-Agent, which is why it is easy to miss\n  on a probe. It is the only security/compliance surface Zoca publishes — zoca.com/security, /trust and /compliance\n  all 404.\ncertifications:\n- HIPAA\nin_progress:\n- GDPR\ncertification_detail:\n- name: HIPAA\n  status: Compliant\n- name: GDPR\n  status: Coming soon\nnot_claimed:\n- SOC 2\n- ISO 27001\n- PCI DSS\n- FedRAMP\n- CSA STAR\ncontrol_families:\n- Product security\n- Data security\n- Network security\n- App security\n- Endpoint security\n- Corporate security\npolicies_published:\n  count: 37+\n  examples:\n  - Operation Security Policy\n  - Business Continuity & Disaster Recovery Policy\n  - Access\
  \ Control Policy\n  - Compliance Policy\n  - Risk Assessment & Management Policy\n  - HR Security Procedure\nsubprocessors_listed: true\nvulnerability_disclosure:\n  published: false\n  note: No security contact, security.txt, bug-bounty programme or responsible-disclosure policy is linked from\n    the trust centre or anywhere on zoca.com.\nevidence:\n- url: https://trust.zoca.com/\n  http_status: 200\n  ua: browser UA required; default curl UA gets CloudFront 403\n  keywords:\n  - HIPAA Compliant\n  - GDPR Coming soon\n  - Trust Center\n  - Sprinto\n- url: https://zoca.com/security\n  http_status: 404\n- url: https://zoca.com/compliance\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/security/zoca-trust-center.yml
summary_line: HIPAA
tags:
- Company
- Artificial Intelligence
- Marketing
- Beauty and Wellness
- Local Business
- AI Agents
- Appointments
- Scheduling
- Booking
- Local SEO
- Google Business Profile
- Social Media
- Salon Software
- Spa
- SaaS
- Lead Generation
- Customer Retention
- Small Business
trust_url: https://trust.zoca.com/
---
