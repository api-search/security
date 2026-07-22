---
api_specs:
- filename: synack-monolith-v1-openapi.yaml
  format: yaml
  label: Synack Enterprise API (Monolith v1)
  slug: synack-enterprise-api-monolith-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v1-openapi.yaml
- filename: synack-monolith-v2-openapi.yaml
  format: yaml
  label: Synack Client API (Monolith v2)
  slug: synack-client-api-monolith-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v2-openapi.yaml
- filename: synack-assessment-v1-openapi.yaml
  format: yaml
  label: Synack Assessment Service
  slug: synack-assessment-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-assessment-v1-openapi.yaml
- filename: synack-asset-v2-openapi.yaml
  format: yaml
  label: Synack Asset Service
  slug: synack-asset-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-v2-openapi.yaml
- filename: synack-asset-discovery-openapi.yaml
  format: yaml
  label: Synack Asset Discovery Service
  slug: synack-asset-discovery-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-discovery-openapi.yaml
- filename: synack-mission-v2-openapi.yaml
  format: yaml
  label: Synack Mission Service v2
  slug: synack-mission-service-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-mission-v2-openapi.yaml
- filename: synack-vulns-openapi.yaml
  format: yaml
  label: Synack Vulnerability Service
  slug: synack-vulnerability-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-vulns-openapi.yaml
- filename: synack-tagging-openapi.yaml
  format: yaml
  label: Synack Tagging Service
  slug: synack-tagging-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-tagging-openapi.yaml
- filename: synack-streaming-openapi.yaml
  format: yaml
  label: Synack Streaming Service
  slug: synack-streaming-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-streaming-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: synack.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: synack.us
  spf: true
hosts:
- cert_expires: Aug 22 22:25:43 2026 GMT
  host: www.synack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 06:05:33 2026 GMT
  host: client.synack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:15:38 2026 GMT
  host: client.synack.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Synack
provider_slug: synack
slug: synack-domain-security
source_filename: synack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: client.synack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: client.synack.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synack.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: synack.us\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/security/synack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Penetration Testing
- Vulnerability Management
- Attack Surface Management
- Crowdsourced Security
- Compliance
- API
---
