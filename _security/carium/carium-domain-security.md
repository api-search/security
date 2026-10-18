---
api_specs:
- filename: carium-caredb-api-openapi.yml
  format: yaml
  label: Carium Caredb API
  slug: carium-caredb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-caredb-api-openapi.yml
- filename: carium-carium-api-api-openapi.yml
  format: yaml
  label: Carium Carium API
  slug: carium-carium-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-carium-api-api-openapi.yml
- filename: carium-carium-inc-api-openapi.yml
  format: yaml
  label: Carium Carium Inc API
  slug: carium-carium-inc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-carium-inc-api-openapi.yml
- filename: carium-identity-api-openapi.yml
  format: yaml
  label: Carium Identity API
  slug: carium-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-identity-api-openapi.yml
- filename: carium-lachesis-api-openapi.yml
  format: yaml
  label: Carium Lachesis API
  slug: carium-lachesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-lachesis-api-openapi.yml
- filename: carium-overlord-api-openapi.yml
  format: yaml
  label: Carium Overlord API
  slug: carium-overlord-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-overlord-api-openapi.yml
- filename: carium-showboat-api-openapi.yml
  format: yaml
  label: Carium Showboat API
  slug: carium-showboat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/openapi/carium-showboat-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carium.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.carium.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carium
provider_slug: carium
slug: carium-domain-security
source_filename: carium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: carium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carium/refs/heads/main/security/carium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- VirtualCare
- Remote Monitoring
- Patient Engagement
- Health Tech
- Company
---
