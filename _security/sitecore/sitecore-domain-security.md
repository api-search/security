---
api_specs:
- filename: sitecore-xm-cloud-rest-api-openapi.yml
  format: yaml
  label: Sitecore XM Cloud REST API
  slug: xm-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-xm-cloud-rest-api-openapi.yml
- filename: sitecore-cdp-rest-api-openapi.yml
  format: yaml
  label: Sitecore CDP REST API
  slug: cdp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-cdp-rest-api-openapi.yml
- filename: sitecore-cdp-stream-api-asyncapi.yml
  format: yaml
  label: Sitecore CDP Stream API
  slug: cdp-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/asyncapi/sitecore-cdp-stream-api-asyncapi.yml
- filename: sitecore-personalize-rest-api-openapi.yml
  format: yaml
  label: Sitecore Personalize REST API
  slug: personalize-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-personalize-rest-api-openapi.yml
- filename: sitecore-content-hub-rest-api-openapi.yml
  format: yaml
  label: Sitecore Content Hub REST API
  slug: content-hub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-content-hub-rest-api-openapi.yml
- filename: sitecore-ordercloud-api-openapi.yml
  format: yaml
  label: Sitecore OrderCloud API
  slug: ordercloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-ordercloud-api-openapi.yml
- filename: sitecore-discover-api-openapi.yml
  format: yaml
  label: Sitecore Discover API
  slug: discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-discover-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sitecore.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sitecorecloud.io
  spf: true
hosts:
- cert_expires: Aug 15 08:11:35 2026 GMT
  host: doc.sitecore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:04:59 2026 GMT
  host: edge.sitecorecloud.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:04:59 2026 GMT
  host: xmapps-api.sitecorecloud.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sitecore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sitecore, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: sitecore
provider_slug: sitecore
slug: sitecore-domain-security
source_filename: sitecore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doc.sitecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 08:11:35 2026 GMT\n  hsts: null\n- host: edge.sitecorecloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:04:59 2026 GMT\n  hsts: null\n- host: xmapps-api.sitecorecloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:04:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sitecore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sitecorecloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/security/sitecore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
