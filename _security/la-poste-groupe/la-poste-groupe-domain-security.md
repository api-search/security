---
api_specs:
- filename: la-poste-groupe-suivi-openapi.json
  format: json
  label: La Poste Suivi v2
  slug: la-poste-suivi-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-suivi-openapi.json
- filename: la-poste-groupe-digiposte-openapi.json
  format: json
  label: Digiposte v3
  slug: digiposte-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-digiposte-openapi.json
- filename: la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
  format: json
  label: Lettre recommandee en ligne v1
  slug: lettre-recommandee-en-ligne-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
- filename: la-poste-groupe-open-data-openapi.json
  format: json
  label: La Poste Open Data v1
  slug: la-poste-open-data-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-open-data-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lapostegroupe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: laposte.fr
  spf: true
hosts:
- cert_expires: Nov 22 07:01:18 2026 GMT
  host: www.lapostegroupe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 10:01:31 2026 GMT
  host: developer.laposte.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 10:01:31 2026 GMT
  host: api.laposte.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Poste Groupe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Poste Groupe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: La Poste Groupe
provider_slug: la-poste-groupe
slug: la-poste-groupe-domain-security
source_filename: la-poste-groupe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lapostegroupe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:01:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.laposte.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:01:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.laposte.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:01:31 2026 GMT\n  hsts: null\ndomains:\n- domain: lapostegroupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: laposte.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes:\n  api_laposte_fr_hsts: >-\n    The automated probe recorded hsts: null for api.laposte.fr because the host root\n    does not answer with the header. A live GET of a real API path\n    (https://api.laposte.fr/suivi/v2/idships/...\
  \ , HTTP 401, 2026-09-02) DID return\n    strict-transport-security: max-age=31536000; includeSubDomains. HSTS is present\n    on the API surface itself.\n  hosts_not_probed: >-\n    ws.colissimo.fr, data.laposte.fr and api.digiposte.fr are real hosts in this\n    estate that this run's automated probe did not cover. Both Colissimo WSDLs and\n    the data.laposte.fr OpenAPI and .well-known documents were fetched over HTTPS\n    successfully on 2026-09-02, so all three serve TLS; their HSTS, CAA and DNSSEC\n    posture is unmeasured rather than absent.\n  dmarc_finding: >-\n    laposte.fr - the domain carrying the developer portal, the API gateway and the\n    CERT contact address - publishes DMARC p=none (monitor only), while\n    lapostegroupe.com publishes p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/security/la-poste-groupe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Package Tracking
- Postal
- Addresses
- Geocoding
- Open Data
- Document Management
- Identity
- Government
- France
---
