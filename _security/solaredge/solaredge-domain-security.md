---
api_specs:
- filename: solaredge-account-api-openapi.yml
  format: yaml
  label: Solaredge Account API
  slug: solaredge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-account-api-openapi.yml
- filename: solaredge-equipment-api-openapi.yml
  format: yaml
  label: Solaredge Equipment API
  slug: solaredge-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-equipment-api-openapi.yml
- filename: solaredge-sites-api-openapi.yml
  format: yaml
  label: Solaredge Sites API
  slug: solaredge-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-sites-api-openapi.yml
- filename: solaredge-storage-api-openapi.yml
  format: yaml
  label: Solaredge Storage API
  slug: solaredge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-storage-api-openapi.yml
- filename: solaredge-version-api-openapi.yml
  format: yaml
  label: Solaredge Version API
  slug: solaredge-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "Digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solaredge.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 18:25:40 2026 GMT
  host: api-docs.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: monitoringapi.solaredge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solaredge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solaredge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solaredge
provider_slug: solaredge
slug: solaredge-domain-security
source_filename: solaredge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: api-docs.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:25:40 2026 GMT\n  hsts: null\n- host: monitoringapi.solaredge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: solaredge.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/security/solaredge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Solar Energy
- Photovoltaic
- Energy Monitoring
- IoT
- Renewable Energy
- Inverters
- Energy Storage
---
