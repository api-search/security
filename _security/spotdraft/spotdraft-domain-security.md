---
api_specs:
- filename: spotdraft-openapi.yml
  format: yaml
  label: SpotDraft Public API
  slug: spotdraft-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotdraft/refs/heads/main/openapi/spotdraft-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spotdraft.com
  spf: true
hosts:
- cert_expires: Aug 17 07:38:47 2026 GMT
  host: www.spotdraft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:49:26 2026 GMT
  host: api.spotdraft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:51:50 2026 GMT
  host: api.us.spotdraft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotdraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpotDraft, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpotDraft
provider_slug: spotdraft
slug: spotdraft-domain-security
source_filename: spotdraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spotdraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:38:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spotdraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:49:26 2026 GMT\n  hsts: null\n- host: api.us.spotdraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spotdraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotdraft/refs/heads/main/security/spotdraft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Lifecycle Management
- CLM
- Contracts
- Legal Tech
- E-Signature
- Clickwrap
- Workflows
- Approvals
- Negotiation
- Templates
- Counterparties
- Obligations
- Analytics
- Webhooks
- AI
- SaaS
- Bangalore
---
