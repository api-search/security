---
api_specs:
- filename: podkitapp-com-admin-api-openapi.yml
  format: yaml
  label: podkitapp-com Admin API
  slug: podkitapp-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-admin-api-openapi.yml
- filename: podkitapp-com-episodes-api-openapi.yml
  format: yaml
  label: podkitapp-com Episodes API
  slug: podkitapp-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-episodes-api-openapi.yml
- filename: podkitapp-com-podcasts-api-openapi.yml
  format: yaml
  label: podkitapp-com Podcasts API
  slug: podkitapp-com-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-podcasts-api-openapi.yml
- filename: podkitapp-com-search-api-openapi.yml
  format: yaml
  label: podkitapp-com Search API
  slug: podkitapp-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-search-api-openapi.yml
- filename: podkitapp-com-usage-api-openapi.yml
  format: yaml
  label: podkitapp-com Usage API
  slug: podkitapp-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: podkitapp.com
  spf: true
hosts:
- cert_expires: Dec 10 07:55:38 2026 GMT
  host: podkitapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Podkitapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for podkitapp-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: podkitapp-com
provider_slug: podkitapp-com
slug: podkitapp-com-domain-security
source_filename: podkitapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podkitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 07:55:38 2026 GMT\n  hsts: false\ndomains:\n- domain: podkitapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/podkitapp-com/security/podkitapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Podcast
- API
- Data
- Developer
- Audio
---
