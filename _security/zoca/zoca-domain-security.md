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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zoca.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zoca.ai
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: zoca.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: app.zoca.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.zoca.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: tasks.zoca.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: public.zoca.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoca, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zoca
provider_slug: zoca
slug: zoca-domain-security
source_filename: zoca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zoca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: app.zoca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: api.zoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: tasks.zoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: public.zoca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\ndomains:\n- domain: zoca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zoca.ai\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: none\nnote: Hosts probed live. api.zoca.ai and zoca.com serve NO HSTS header; tasks.zoca.ai and public.zoca.com serve\n  max-age=63072000; includeSubDomains. Neither registrable domain (zoca.com, zoca.ai) has DNSSEC or a CAA record,\n  and zoca.ai publishes DMARC p=none (monitor only) while zoca.com publishes p=quarantine.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/security/zoca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
