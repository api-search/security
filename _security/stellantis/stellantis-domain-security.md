---
api_specs:
- filename: stellantis-data-treatment-openapi.yml
  format: yaml
  label: Stellantis Data Treatment API
  slug: stellantis-data-treatment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellantis/refs/heads/main/openapi/_original/stellantis-data-treatment-openapi.yml
- filename: stellantis-data-treatment-system-openapi.yml
  format: yaml
  label: Stellantis Data Treatment System API
  slug: stellantis-data-treatment-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellantis/refs/heads/main/openapi/_original/stellantis-data-treatment-system-openapi.yml
- filename: stellantis-data-treatment-openapi.yml
  format: yaml
  label: Stellantis Data Treatment API
  slug: stellantis-data-treatment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellantis/refs/heads/main/openapi/_original/stellantis-data-treatment-openapi.yml
- filename: stellantis-data-treatment-system-openapi.yml
  format: yaml
  label: Stellantis Data Treatment System API
  slug: stellantis-data-treatment-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellantis/refs/heads/main/openapi/_original/stellantis-data-treatment-system-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stellantis.com
  spf: true
hosts:
- cert_expires: Dec  2 08:33:24 2026 GMT
  host: www.stellantis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stellantis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellantis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stellantis
provider_slug: stellantis
slug: stellantis-domain-security
source_filename: stellantis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stellantis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 08:33:24 2026 GMT\n  hsts: null\ndomains:\n- domain: stellantis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellantis/refs/heads/main/security/stellantis-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Automotive
- Manufacturing
- Mobility
- Sustainability
---
