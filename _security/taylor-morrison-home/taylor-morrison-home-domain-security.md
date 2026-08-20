---
api_specs:
- filename: taylor-morrison-home-communities-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Communities API
  slug: taylor-morrison-home-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-communities-api-openapi.yml
- filename: taylor-morrison-home-design-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Design API
  slug: taylor-morrison-home-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-design-api-openapi.yml
- filename: taylor-morrison-home-floor-plans-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Floor Plans API
  slug: taylor-morrison-home-floor-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-floor-plans-api-openapi.yml
- filename: taylor-morrison-home-homes-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Homes API
  slug: taylor-morrison-home-homes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-homes-api-openapi.yml
- filename: taylor-morrison-home-lots-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Lots API
  slug: taylor-morrison-home-lots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-lots-api-openapi.yml
- filename: taylor-morrison-home-reservations-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Reservations API
  slug: taylor-morrison-home-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-reservations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: taylormorrison.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: taylormorrisonfunding.com
  spf: false
hosts:
- cert_expires: Sep 13 22:36:17 2026 GMT
  host: www.taylormorrison.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.taylormorrisonfunding.com
  https: false
kind: domain-security
layout: security
method: probed
name: Taylor Morrison Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for taylor-morrison-home, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: taylor-morrison-home
provider_slug: taylor-morrison-home
slug: taylor-morrison-home-domain-security
source_filename: taylor-morrison-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taylormorrison.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:36:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.taylormorrisonfunding.com\n  https: false\ndomains:\n- domain: taylormorrison.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: taylormorrisonfunding.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/security/taylor-morrison-home-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Homebuilding
- Real-Estate
- Fortune 1000
- New Homes
- Communities
- Mortgage
---
