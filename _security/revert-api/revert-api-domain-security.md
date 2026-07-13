---
api_specs:
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified CRM API
  slug: revert-api-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Chat API
  slug: revert-api-unified-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Ticketing API
  slug: revert-api-unified-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Connection Management API
  slug: revert-api-connection-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Metadata API
  slug: revert-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Passthrough Proxy API
  slug: revert-api-passthrough-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Accounting API
  slug: revert-api-unified-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified ATS API
  slug: revert-api-unified-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
description: ''
domains:
- apexARecord: false
  caa: []
  dmarc: unknown
  dnssec: false
  domain: revert.dev
  nameservers:
  - dns1.registrar-servers.com
  - dns2.registrar-servers.com
  note: Domain is still registered but parked at registrar default nameservers with no A records and no application hosts. Consistent with the hosted service having been wound down after the Ampersand transition.
  registered: true
  soaOnly: true
  spf: unknown
hosts:
- host: api.revert.dev
  https: false
  note: NXDOMAIN - no A record. Historical hosted REST API base; now offline.
  resolves: false
- host: docs.revert.dev
  https: false
  note: NXDOMAIN - no A record. Historical hosted documentation; now offline.
  resolves: false
- host: www.revert.dev
  https: false
  note: NXDOMAIN - no A record.
  resolves: false
- host: github.com
  https: true
  note: Live source of truth - github.com/revertinc/revert (AGPL-3.0). API definition and backend routes read here.
  resolves: true
kind: domain-security
layout: security
method: probed
name: Revert Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revert, probed live across 4 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Revert
provider_slug: revert-api
slug: revert-api-domain-security
source_filename: revert-api-domain-security.yml
source_heading: Domain Security
source_url: https://github.com/revertinc/revert
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (2026-07-12)\nserviceStatus: retired\nstatusNote: >-\n  Revert has joined Ampersand. The hosted Revert domains no longer resolve to any\n  A record - the apex revert.dev returns only an SOA at Namecheap default\n  nameservers (dns1/dns2.registrar-servers.com) and the www/api/docs subdomains\n  return NXDOMAIN. The hosted API (api.revert.dev), app, and docs (docs.revert.dev)\n  are therefore offline as of this probe. The open-source repository on GitHub\n  remains live and is the grounded source for this catalog entry.\nhosts:\n- host: api.revert.dev\n  resolves: false\n  https: false\n  note: NXDOMAIN - no A record. Historical hosted REST API base; now offline.\n- host: docs.revert.dev\n  resolves: false\n  https: false\n  note: NXDOMAIN - no A record. Historical hosted documentation; now offline.\n- host: www.revert.dev\n  resolves: false\n  https: false\n  note: NXDOMAIN\
  \ - no A record.\n- host: github.com\n  resolves: true\n  https: true\n  note: Live source of truth - github.com/revertinc/revert (AGPL-3.0). API definition and backend routes read here.\ndomains:\n- domain: revert.dev\n  registered: true\n  nameservers:\n  - dns1.registrar-servers.com\n  - dns2.registrar-servers.com\n  apexARecord: false\n  soaOnly: true\n  dnssec: false\n  caa: []\n  spf: unknown\n  dmarc: unknown\n  note: >-\n    Domain is still registered but parked at registrar default nameservers with no\n    A records and no application hosts. Consistent with the hosted service having\n    been wound down after the Ampersand transition.\nsources:\n- https://github.com/revertinc/revert\n- https://dns.google/resolve?name=revert.dev\n- https://cloudflare-dns.com/dns-query?name=revert.dev\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/security/revert-api-domain-security.yml
summary_line: DMARC
tags:
- Unified API
- Embedded iPaaS
- Integrations
- Product Integrations
- Open Source
- CRM Integrations
- Connectors
- API Integration
---
