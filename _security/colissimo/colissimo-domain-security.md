---
api_specs:
- filename: colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api-openapi.yml
  format: yaml
  label: Colissimo Description et exemples des méthodes du WS SLS API
  slug: colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api-openapi.yml
- filename: colissimo-g-n-ration-de-bordereau-de-d-pot-api-openapi.yml
  format: yaml
  label: Colissimo Génération de bordereau de dépot API
  slug: colissimo-g-n-ration-de-bordereau-de-d-pot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-g-n-ration-de-bordereau-de-d-pot-api-openapi.yml
- filename: colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api-openapi.yml
  format: yaml
  label: 'Colissimo SlsInternalService : Services destinés aux applications internes API'
  slug: colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api-openapi.yml
- filename: colissimo-slsservicews-documentation-api-openapi.yml
  format: yaml
  label: 'Colissimo SlsServiceWS : documentation API'
  slug: colissimo-slsservicews-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-slsservicews-documentation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: colissimo.fr
  spf: true
hosts:
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: www.colissimo.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Colissimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colissimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Colissimo
provider_slug: colissimo
slug: colissimo-domain-security
source_filename: colissimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colissimo.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: colissimo.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/security/colissimo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Shipping
- Logistics
- Parcel
- Labels
- Pickup Points
- France
---
