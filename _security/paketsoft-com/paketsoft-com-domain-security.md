---
api_specs:
- filename: paketsoft-com-katalog-api-openapi.yml
  format: yaml
  label: PaketSoft Katalog API
  slug: paketsoft-com-katalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-katalog-api-openapi.yml
- filename: paketsoft-com-kuponlar-api-openapi.yml
  format: yaml
  label: PaketSoft Kuponlar API
  slug: paketsoft-com-kuponlar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-kuponlar-api-openapi.yml
- filename: paketsoft-com-m-teriler-api-openapi.yml
  format: yaml
  label: PaketSoft Müşteriler API
  slug: paketsoft-com-m-teriler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-m-teriler-api-openapi.yml
- filename: paketsoft-com-r-nler-api-openapi.yml
  format: yaml
  label: PaketSoft Ürünler API
  slug: paketsoft-com-r-nler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-r-nler-api-openapi.yml
- filename: paketsoft-com-rapor-api-openapi.yml
  format: yaml
  label: PaketSoft Rapor API
  slug: paketsoft-com-rapor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-rapor-api-openapi.yml
- filename: paketsoft-com-sipari-ler-api-openapi.yml
  format: yaml
  label: PaketSoft Siparişler API
  slug: paketsoft-com-sipari-ler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-sipari-ler-api-openapi.yml
- filename: paketsoft-com-webhooklar-api-openapi.yml
  format: yaml
  label: PaketSoft Webhooklar API
  slug: paketsoft-com-webhooklar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-webhooklar-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paketsoft.com
  spf: true
hosts:
- cert_expires: Jan 27 09:43:49 2027 GMT
  host: paketsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PaketSoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PaketSoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PaketSoft
provider_slug: paketsoft-com
slug: paketsoft-com-domain-security
source_filename: paketsoft-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paketsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 09:43:49 2027 GMT\n  hsts: false\ndomains:\n- domain: paketsoft.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/paketsoft-com/security/paketsoft-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
