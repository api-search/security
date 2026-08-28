---
api_specs:
- filename: metabolon-portal-api-openapi.yml
  format: yaml
  label: Metabolon Portal API
  slug: metabolon-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-portal-api-openapi.yml
- filename: metabolon-discovery-panels-api-openapi.yml
  format: yaml
  label: Metabolon Discovery Panels API
  slug: metabolon-discovery-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-discovery-panels-api-openapi.yml
- filename: metabolon-pathway-explorer-api-openapi.yml
  format: yaml
  label: Metabolon Pathway Explorer API
  slug: metabolon-pathway-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-pathway-explorer-api-openapi.yml
- filename: metabolon-heatmap-api-openapi.yml
  format: yaml
  label: Metabolon Heatmap API
  slug: metabolon-heatmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-heatmap-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metabolon.com
  spf: false
hosts:
- cert_expires: Oct 28 02:32:01 2026 GMT
  host: www.metabolon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: portal-api.prod.metabolon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: discovery.prod.metabolon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metabolon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metabolon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Metabolon
provider_slug: metabolon
slug: metabolon-domain-security
source_filename: metabolon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 02:32:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal-api.prod.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\n- host: discovery.prod.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metabolon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/security/metabolon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Metabolomics
- Life Sciences
- Bioinformatics
- Multiomics
- Biotechnology
- Drug Discovery
- Precision Medicine
- Microbiome
- Biomarkers
- Contract Research
- Laboratory
---
