---
api_specs:
- filename: macrometa-gdn-openapi-original.json
  format: json
  label: Macrometa Global Data Network (GDN) API
  slug: macrometa-global-data-network-gdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-gdn-openapi-original.json
- filename: macrometa-photoniq-eds-openapi-original.json
  format: json
  label: PhotonIQ Event Delivery Service (EDS) API
  slug: photoniq-event-delivery-service-eds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-eds-openapi-original.json
- filename: macrometa-photoniq-est-openapi-original.json
  format: json
  label: PhotonIQ Edge Side Tagging (EST) API
  slug: photoniq-edge-side-tagging-est-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-est-openapi-original.json
- filename: macrometa-photoniq-faas-openapi-original.json
  format: json
  label: PhotonIQ Function as a Service (FaaS) API
  slug: photoniq-function-as-a-service-faas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-faas-openapi-original.json
- filename: macrometa-photoniq-fps-openapi-original.json
  format: json
  label: PhotonIQ Fingerprint (FPS) API
  slug: photoniq-fingerprint-fps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-fps-openapi-original.json
- filename: macrometa-photoniq-hss-openapi-original.json
  format: json
  label: PhotonIQ HyperSearch (HSS) API
  slug: photoniq-hypersearch-hss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-hss-openapi-original.json
- filename: macrometa-photoniq-prerender-openapi-original.json
  format: json
  label: PhotonIQ Prerender Service API
  slug: photoniq-prerender-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-prerender-openapi-original.json
- filename: macrometa-photoniq-vwrs-openapi-original.json
  format: json
  label: PhotonIQ Virtual Waiting Rooms (VWRS) API
  slug: photoniq-virtual-waiting-rooms-vwrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-vwrs-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: macrometa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: macrometa.io
  spf: false
hosts:
- cert_expires: Aug 25 10:29:44 2026 GMT
  host: www.macrometa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api-play.paas.macrometa.io
  https: false
- host: api-demo-est.paas.macrometa.io
  https: false
kind: domain-security
layout: security
method: probed
name: Macrometa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macrometa, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Macrometa
provider_slug: macrometa
slug: macrometa-domain-security
source_filename: macrometa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.macrometa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:29:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-play.paas.macrometa.io\n  https: false\n- host: api-demo-est.paas.macrometa.io\n  https: false\ndomains:\n- domain: macrometa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: macrometa.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/security/macrometa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Edge Computing
- Database
- NoSQL
- Serverless
- Streaming
- Stream Processing
- Real Time
- Web Performance
- CDN
- Search
- Artificial Intelligence
- API
---
