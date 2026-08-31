---
api_specs:
- filename: america-movil-check-sim-swap-api-openapi.yml
  format: yaml
  label: América Móvil Check SIM swap API
  slug: america-movil-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-check-sim-swap-api-openapi.yml
- filename: america-movil-device-locations-api-openapi.yml
  format: yaml
  label: América Móvil Device Locations API
  slug: america-movil-device-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-device-locations-api-openapi.yml
- filename: america-movil-location-verification-api-openapi.yml
  format: yaml
  label: América Móvil Location verification API
  slug: america-movil-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-location-verification-api-openapi.yml
- filename: america-movil-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: América Móvil Retrieve SIM swap date API
  slug: america-movil-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-retrieve-sim-swap-date-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: americamovil.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telcel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_note: pct=100, fo=1, rua/ruf reporting to OnDMARC and Cisco DMP
  dmarc_policy: reject
  dnssec: false
  domain: claro.com.br
  spf: true
- caa: []
  dmarc: false
  dmarc_note: No _dmarc record. The domain that hosts the developer marketplace, the registration flow and the login is the one domain in the estate with no DMARC policy — a phishing surface aimed squarely at API customers.
  dnssec: false
  domain: claroinsight.com.br
  spf: true
hosts:
- cert_expires: Oct 19 08:08:32 2026 GMT
  host: www.americamovil.com
  hsts: false
  https: true
  role: corporate / investor relations
  tls_version: TLSv1.3
- cert_expires: Aug  8 23:59:59 2026 GMT
  host: www.telcel.com
  hsts: null
  https: true
  role: Mexico operating company
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.claro.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Brazil operating company
  tls_version: TLSv1.3
- anonymous_status: 403
  cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.claro.com.br
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: production API gateway edge (CloudFront)
  tls_version: TLSv1.3
- anonymous_status: 404
  cert_expires: Jan  6 23:59:59 2027 GMT
  host: api-sandbox.claro.com.br
  hsts: false
  https: true
  role: sandbox API edge
  tls_version: TLSv1.3
- anonymous_status: 200
  cert_expires: Jan 11 23:59:59 2027 GMT
  host: www.claroinsight.com.br
  hsts: false
  https: true
  role: Claro Insight API marketplace (the group's only developer portal)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: America Movil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for América Móvil, probed live across 6 host(s) and 4 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: América Móvil
provider_slug: america-movil
slug: america-movil-domain-security
source_filename: america-movil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every apis.yml host and every OpenAPI servers[]\n  host, extended by hand to cover the API edge, the sandbox edge, the developer\n  marketplace and the .com.br registrable domains the automated pass skipped.\nhosts:\n- host: www.americamovil.com\n  role: corporate / investor relations\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 08:08:32 2026 GMT\n  hsts: false\n- host: www.telcel.com\n  role: Mexico operating company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 23:59:59 2026 GMT\n  hsts: null\n- host: www.claro.com.br\n  role: Brazil operating company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.claro.com.br\n  role: production API gateway edge (CloudFront)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n\
  \  hsts_include_subdomains: true\n  anonymous_status: 403\n- host: api-sandbox.claro.com.br\n  role: sandbox API edge\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n  anonymous_status: 404\n- host: www.claroinsight.com.br\n  role: Claro Insight API marketplace (the group's only developer portal)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\n  anonymous_status: 200\ndomains:\n- domain: americamovil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: telcel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: claro.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_note: 'pct=100, fo=1, rua/ruf reporting to OnDMARC and Cisco DMP'\n- domain: claroinsight.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_note: >-\n    No _dmarc record. The\
  \ domain that hosts the developer marketplace, the\n    registration flow and the login is the one domain in the estate with no DMARC\n    policy — a phishing surface aimed squarely at API customers.\nobservations:\n- Strong e-mail authentication on the brand domains (SPF + DMARC p=reject) but none on claroinsight.com.br.\n- No CAA record on any domain — any CA may issue for these names.\n- No DNSSEC anywhere in the estate.\n- HSTS is enforced on the production API edge and the Brazilian consumer site, but not on the sandbox edge or the developer marketplace.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/security/america-movil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Mexico
- Latin America
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Device Location
- Broadband
- 5G
- Carrier
---
