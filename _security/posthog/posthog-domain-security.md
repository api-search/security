---
api_specs:
- filename: posthog-openapi.yml
  format: yaml
  label: PostHog API
  slug: posthog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posthog/refs/heads/main/openapi/posthog-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: posthog.com
  spf: true
hosts:
- cert_expires: Aug 12 16:51:09 2026 GMT
  host: posthog.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:17:38 2026 GMT
  host: app.posthog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Posthog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostHog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PostHog
provider_slug: posthog
slug: posthog-domain-security
source_filename: posthog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: posthog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.posthog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: posthog.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posthog/refs/heads/main/security/posthog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- A/B Testing
- Analytics
- Feature Flags
- Open Source
- Product Analytics
- Session Recording
---
