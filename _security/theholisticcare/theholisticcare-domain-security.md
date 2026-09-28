---
api_specs:
- filename: theholisticcare-health-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Health API
  slug: theholisticcare-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-health-api-openapi.yml
- filename: theholisticcare-resources-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Resources API
  slug: theholisticcare-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-resources-api-openapi.yml
- filename: theholisticcare-search-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Search API
  slug: theholisticcare-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theholisticcare.com
  spf: true
hosts:
- cert_expires: Dec 23 06:15:13 2026 GMT
  host: api.theholisticcare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Theholisticcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Holistic Care — THC Open Mindfulness API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Holistic Care — THC Open Mindfulness API
provider_slug: theholisticcare
slug: theholisticcare-domain-security
source_filename: theholisticcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.theholisticcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 06:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: theholisticcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/security/theholisticcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mindfulness
- Education
- Health
- OpenAPI
- PublicAPI
- Free
---
