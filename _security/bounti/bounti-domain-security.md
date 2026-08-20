---
api_specs:
- filename: bounti-llms-full-txt-api-openapi.yml
  format: yaml
  label: Bounti Llms Full.txt API
  slug: bounti-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/openapi/bounti-llms-full-txt-api-openapi.yml
- filename: bounti-llms-txt-api-openapi.yml
  format: yaml
  label: Bounti Llms.txt API
  slug: bounti-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/openapi/bounti-llms-txt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bounti.ai
  note: DMARC policy is p=none (monitor only) — it publishes a record but enforces nothing. No CAA records and no DNSSEC.
  spf: true
hosts:
- cert_expires: Nov  9 00:49:15 2026 GMT
  host: bounti.ai
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 05:28:07 2026 GMT
  host: claw.bounti.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: B.Claw application host. Response headers also carry x-frame-options DENY, x-content-type-options nosniff, referrer-policy strict-origin-when-cross-origin, cross-origin-resource-policy same-origin, permissions-policy camera=() geolocation=() and cache-control no-store — a materially stronger header posture than the marketing apex.
  server: Google Frontend
- cert_expires: Sep 20 04:16:34 2026 GMT
  host: re.bounti.ai
  hsts: false
  https: true
  note: Real-estate product sign-in host; no Strict-Transport-Security header observed.
- host: api.bounti.ai
  https: true
  note: Resolves and terminates TLS but returns HTTP 404 with an empty body for every path probed.
kind: domain-security
layout: security
method: probed
name: Bounti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounti, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bounti
provider_slug: bounti
slug: bounti-domain-security
source_filename: bounti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (0-working/probe-domain-security.py, plus hand probes of the product subdomains)\nhosts:\n- host: bounti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n  hsts_include_subdomains: false\n- host: claw.bounti.ai\n  https: true\n  cert_expires: Oct 16 05:28:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Google Frontend\n  note: >-\n    B.Claw application host. Response headers also carry x-frame-options DENY, x-content-type-options\n    nosniff, referrer-policy strict-origin-when-cross-origin, cross-origin-resource-policy\n    same-origin, permissions-policy camera=() geolocation=() and cache-control no-store — a\n    materially stronger header posture than the marketing apex.\n- host: re.bounti.ai\n  https: true\n  cert_expires: Sep 20 04:16:34 2026 GMT\n\
  \  hsts: false\n  note: Real-estate product sign-in host; no Strict-Transport-Security header observed.\n- host: api.bounti.ai\n  https: true\n  note: Resolves and terminates TLS but returns HTTP 404 with an empty body for every path probed.\ndomains:\n- domain: bounti.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    DMARC policy is p=none (monitor only) — it publishes a record but enforces nothing. No CAA\n    records and no DNSSEC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/security/bounti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Artificial Intelligence
- Marketing
- Sales Enablement
- Virtual Staging
- Content Generation
- AI Agents
---
