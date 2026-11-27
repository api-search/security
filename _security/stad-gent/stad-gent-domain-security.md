---
api_specs:
- filename: stad-gent-catalog-api-openapi.yml
  format: yaml
  label: Stad Gent Catalog API
  slug: stad-gent-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stad-gent/openapi/stad-gent-catalog-api-openapi.yml
- filename: stad-gent-dataset-api-openapi.yml
  format: yaml
  label: Stad Gent Dataset API
  slug: stad-gent-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stad-gent/openapi/stad-gent-dataset-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stad.gent
  spf: true
hosts:
- cert_expires: Dec 17 20:39:56 2026 GMT
  host: data.stad.gent
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stad Gent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stad Gent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stad Gent
provider_slug: stad-gent
slug: stad-gent-domain-security
source_filename: stad-gent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.stad.gent\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 20:39:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stad.gent\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stad-gent/security/stad-gent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Open Data
- Belgium
- Smart City
- Municipal
- Datasets
---
