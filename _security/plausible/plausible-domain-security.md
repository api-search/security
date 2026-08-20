---
api_specs:
- filename: plausible-customprops-api-openapi.yml
  format: yaml
  label: Plausible CustomProps API
  slug: plausible-customprops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-customprops-api-openapi.yml
- filename: plausible-events-api-openapi.yml
  format: yaml
  label: Plausible Events API
  slug: plausible-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-events-api-openapi.yml
- filename: plausible-goals-api-openapi.yml
  format: yaml
  label: Plausible Goals API
  slug: plausible-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-goals-api-openapi.yml
- filename: plausible-guests-api-openapi.yml
  format: yaml
  label: Plausible Guests API
  slug: plausible-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-guests-api-openapi.yml
- filename: plausible-query-api-openapi.yml
  format: yaml
  label: Plausible Query API
  slug: plausible-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-query-api-openapi.yml
- filename: plausible-sharedlinks-api-openapi.yml
  format: yaml
  label: Plausible SharedLinks API
  slug: plausible-sharedlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sharedlinks-api-openapi.yml
- filename: plausible-sites-api-openapi.yml
  format: yaml
  label: Plausible Sites API
  slug: plausible-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sites-api-openapi.yml
- filename: plausible-teams-api-openapi.yml
  format: yaml
  label: Plausible Teams API
  slug: plausible-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plausible.io
  spf: true
hosts:
- cert_expires: Oct 15 03:03:54 2026 GMT
  host: plausible.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plausible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plausible, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plausible
provider_slug: plausible
slug: plausible-domain-security
source_filename: plausible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plausible.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:03:54 2026 GMT\n  hsts: false\ndomains:\n- domain: plausible.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/security/plausible-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Cookie-Free
- Event Tracking
- GDPR
- Goal Conversions
- Open-Source
- Privacy
- Self-Hosted
- Site Management
- Web Analytics
---
