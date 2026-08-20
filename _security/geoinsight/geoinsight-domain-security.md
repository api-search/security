---
api_specs:
- filename: geoinsight-ogc-api-dggs-openapi.yml
  format: yaml
  label: OGC API - DGGS
  slug: ogc-api-dggs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-ogc-api-dggs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geoinsight.ai
  spf: true
hosts:
- cert_expires: Nov 12 07:12:37 2026 GMT
  host: geoinsight.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.geoinsight.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geoinsight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoInsight, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GeoInsight
provider_slug: geoinsight
slug: geoinsight-domain-security
source_filename: geoinsight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geoinsight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:12:37 2026 GMT\n  hsts: false\n- host: api.geoinsight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: geoinsight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n\n# --- API Evangelist enrichment pass 2026-08-20 (same probed method; adds hosts the script does not\n# --- reach and corrects one HSTS reading the script recorded as null) ---\nx-additional-observations:\n  api_geoinsight_ai_hsts:\n    host: api.geoinsight.ai\n    hsts: true\n    hsts_header: max-age=15724800; includeSubDomains\n    note: >-\n      Recorded as null above because the automated probe uses HEAD, and this API answers HEAD / with\n      404 while answering GET / with 200. Observed on GET https://api.geoinsight.ai/collections?f=json,\n\
  \      HTTP 200: strict-transport-security: max-age=15724800; includeSubDomains. max-age is 182 days,\n      below the 1-year value HSTS preload requires.\n  dead_or_misconfigured_hosts:\n    note: >-\n      Three GeoInsight subdomains resolve and accept TCP 443 but present a self-signed\n      \"O=Acme Co, CN=Kubernetes Ingress Controller Fake Certificate\" - the default certificate an\n      unconfigured ingress-nginx serves. An ordinary client cannot complete the handshake. Behind the\n      bad certificate every path returns a 404. Two of the three are load-bearing: the API's own root\n      document attributes to docs.geoinsight.ai, and the official PyPI package tells users to get their\n      credentials from dashboard.geoinsight.ai.\n    hosts:\n      - host: dggs.geoinsight.ai\n        ip: 62.113.194.100\n        tls: fake-kubernetes-ingress-certificate\n        cert_subject: O=Acme Co, CN=Kubernetes Ingress Controller Fake Certificate\n        cert_not_after: Jul 27 10:31:16 2027\
  \ GMT\n        http_status_all_paths: 404\n        server: nginx\n        note: Host previously recorded as this provider's baseURL. Corrected to api.geoinsight.ai.\n      - host: docs.geoinsight.ai\n        ip: 62.113.194.100\n        tls: fake-kubernetes-ingress-certificate\n        http_status_all_paths: 404\n        server: nginx\n        note: Named in the API root document's own attribution field. Serves nothing.\n      - host: dashboard.geoinsight.ai\n        ip: 64.225.143.189\n        tls: fake-kubernetes-ingress-certificate\n        cert_not_after: Jun  5 16:58:26 2027 GMT\n        http_status_all_paths: 404\n        body: default backend - 404\n        note: >-\n          Named in the official PyPI geoinsight package README as where a GeoInsight Personal Token and\n          API Private Key are issued. Serves nothing, so the documented credential path is unreachable.\n  dggs_io:\n    host: dggs.io\n    https: true\n    note: >-\n      Separate domain, same operator - the site\
  \ footer reads \"Powered by GeoInsight\" and links to\n      geoinsight.ai. Carries the DGGS tooling surface (API tester, zone browser, GeoParquet viewer).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/security/geoinsight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- DGGS
- Discrete Global Grid System
- Earth Observation
- Remote Sensing
- Spatial Data
- GIS
- Artificial Intelligence
- Machine-Learning
- Analysis-ready data
- Spatial Tokens
- Sentinel-2
- Copernicus
- OGC
- STAC
- GeoParquet
- H3
---
