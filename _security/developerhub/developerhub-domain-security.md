---
api_specs:
- filename: developerhub-documentation-api-openapi.yml
  format: yaml
  label: DeveloperHub Documentation API
  slug: developerhub-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-documentation-api-openapi.yml
- filename: developerhub-pages-api-openapi.yml
  format: yaml
  label: DeveloperHub Pages API
  slug: developerhub-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-pages-api-openapi.yml
- filename: developerhub-project-api-openapi.yml
  format: yaml
  label: DeveloperHub Project API
  slug: developerhub-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-project-api-openapi.yml
- filename: developerhub-reader-access-api-openapi.yml
  format: yaml
  label: DeveloperHub Reader Access API
  slug: developerhub-reader-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-reader-access-api-openapi.yml
- filename: developerhub-references-api-openapi.yml
  format: yaml
  label: DeveloperHub References API
  slug: developerhub-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-references-api-openapi.yml
- filename: developerhub-versions-api-openapi.yml
  format: yaml
  label: DeveloperHub Versions API
  slug: developerhub-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-versions-api-openapi.yml
- filename: developerhub-changelog-api-openapi.yml
  format: yaml
  label: DeveloperHub Changelog API
  slug: developerhub-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-changelog-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: developerhub.io
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: developerhub.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 17:33:57 2026 GMT
  host: api.developerhub.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Developerhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeveloperHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeveloperHub
provider_slug: developerhub
slug: developerhub-domain-security
source_filename: developerhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developerhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\n- host: api.developerhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:33:57 2026 GMT\n  hsts: false\ndomains:\n- domain: developerhub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/security/developerhub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Reference
- Developer Portals
- Documentation
- Knowledge Base
- OpenAPI
- Docs as Code
- Model Context Protocol
- Agent Skills
---
