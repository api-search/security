---
api_specs:
- filename: navistone-api-info-api-openapi.yml
  format: yaml
  label: NaviStone API Info API
  slug: navistone-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-api-info-api-openapi.yml
- filename: navistone-campaigns-api-openapi.yml
  format: yaml
  label: NaviStone Campaigns API
  slug: navistone-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-campaigns-api-openapi.yml
- filename: navistone-clients-api-openapi.yml
  format: yaml
  label: NaviStone Clients API
  slug: navistone-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-clients-api-openapi.yml
- filename: navistone-domains-api-openapi.yml
  format: yaml
  label: NaviStone Domains API
  slug: navistone-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-domains-api-openapi.yml
- filename: navistone-geo-targeting-api-openapi.yml
  format: yaml
  label: NaviStone Geo Targeting API
  slug: navistone-geo-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-geo-targeting-api-openapi.yml
- filename: navistone-health-api-openapi.yml
  format: yaml
  label: NaviStone Health API
  slug: navistone-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-health-api-openapi.yml
- filename: navistone-output-api-openapi.yml
  format: yaml
  label: NaviStone Output API
  slug: navistone-output-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-output-api-openapi.yml
- filename: navistone-segments-api-openapi.yml
  format: yaml
  label: NaviStone Segments API
  slug: navistone-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-segments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navistone.com
  spf: true
hosts:
- cert_expires: Sep 20 19:12:43 2026 GMT
  host: www.navistone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.navistone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navistone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NaviStone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NaviStone
provider_slug: navistone
slug: navistone-domain-security
source_filename: navistone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navistone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:12:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.navistone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: navistone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/security/navistone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Direct Mail
- Advertising
- Customer Acquisition
- Audience Targeting
- MarTech
- AdTech
- Postcards
- Retargeting
---
