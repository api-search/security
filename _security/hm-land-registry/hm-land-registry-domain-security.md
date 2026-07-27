---
api_specs:
- filename: hm-land-registry-use-land-property-data-openapi.yml
  format: yaml
  label: Use Land and Property Data API
  slug: use-land-and-property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-use-land-property-data-openapi.yml
- filename: hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json
  format: json
  label: Business Gateway Submit an Application to Change the Land Register API
  slug: business-gateway-submit-an-application-to-change-the-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json
- filename: hm-land-registry-official-search-of-whole-with-data-openapi.yml
  format: yaml
  label: Business Gateway Official Search of Whole (with Priority) with Data API
  slug: business-gateway-official-search-of-whole-with-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-search-of-whole-with-data-openapi.yml
- filename: hm-land-registry-official-copy-document-availability-v2-openapi.json
  format: json
  label: Business Gateway Official Copy Document Availability Service
  slug: business-gateway-official-copy-document-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json
- filename: hm-land-registry-registered-proprietor-names-openapi.json
  format: json
  label: Business Gateway Registered Proprietor Names Service
  slug: business-gateway-registered-proprietor-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-registered-proprietor-names-openapi.json
- filename: hm-land-registry-estimate-completion-date-openapi.yml
  format: yaml
  label: Business Gateway Estimate Completion Date API
  slug: business-gateway-estimate-completion-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-estimate-completion-date-openapi.yml
- filename: hm-land-registry-land-register-api-openapi.yml
  format: yaml
  label: Land Register API
  slug: land-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-land-register-api-openapi.yml
description: ''
domains:
- caa:
  - www-cdn.production.govuk.service.gov.uk.
  - www-gov-uk.map.fastly.net.
  dmarc: false
  dnssec: true
  domain: www.gov.uk
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_detail: v=DMARC1; p=reject; fo=1; aspf=s; adkim=s; pct=100; rua to dmarc-rua@dmarc.service.gov.uk
  dmarc_policy: reject
  dnssec: false
  domain: landregistry.gov.uk
  note: The Business Gateway registrable domain. Strong email posture (DMARC p=reject with strict alignment); no DNSSEC and no CAA.
  spf: true
  spf_detail: v=spf1 ip4:193.110.246.137 include:spf.protection.outlook.com include:spf_a.oracle.com include:spf_c.oracle.com include:spf_c.oraclecloud.com ~all
hosts:
- cert_expires: Dec 28 22:06:14 2026 GMT
  host: www.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: landregistry.data.gov.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 11:14:43 2026 GMT
  host: use-land-property-data.service.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: businessgateway.landregistry.gov.uk
  hsts: null
  https: null
  note: TLS handshake refused without an HMLR-issued client certificate. Mutual TLS is mandatory, which is a stronger transport posture than any HSTS setting — but it also means the host cannot be assessed from outside.
  tls_version: null
- host: bgtest.landregistry.gov.uk
  hsts: null
  https: null
  note: Customer test endpoint. TLS handshake refused without an HMLR-issued client certificate.
  tls_version: null
- host: landregistry.github.io
  hsts: null
  https: true
  note: GitHub Pages host serving the Business Gateway developer pack. Not HMLR-operated infrastructure.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hm Land Registry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HM Land Registry, probed live across 6 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: HM Land Registry
provider_slug: hm-land-registry
slug: hm-land-registry-domain-security
source_filename: hm-land-registry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; Business Gateway hosts probed manually 2026-07-26\nhosts:\n- host: www.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: landregistry.data.gov.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: use-land-property-data.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:14:43 2026 GMT\n  hsts: null\n- host: businessgateway.landregistry.gov.uk\n  https: null\n  tls_version: null\n  hsts: null\n  note: TLS handshake refused without an HMLR-issued client certificate. Mutual TLS is mandatory, which\n    is a stronger transport posture than any HSTS setting — but it also means the host cannot be assessed\n    from outside.\n- host: bgtest.landregistry.gov.uk\n  https: null\n  tls_version: null\n  hsts: null\n\
  \  note: Customer test endpoint. TLS handshake refused without an HMLR-issued client certificate.\n- host: landregistry.github.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: null\n  note: GitHub Pages host serving the Business Gateway developer pack. Not HMLR-operated infrastructure.\ndomains:\n- domain: www.gov.uk\n  dnssec: true\n  caa:\n  - www-cdn.production.govuk.service.gov.uk.\n  - www-gov-uk.map.fastly.net.\n  spf: false\n  dmarc: false\n- domain: data.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: landregistry.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_detail: v=DMARC1; p=reject; fo=1; aspf=s; adkim=s; pct=100; rua to dmarc-rua@dmarc.service.gov.uk\n  spf_detail: v=spf1 ip4:193.110.246.137 include:spf.protection.outlook.com include:spf_a.oracle.com include:spf_c.oracle.com\n    include:spf_c.oraclecloud.com ~all\n  note: The Business Gateway registrable domain. Strong email posture (DMARC p=reject\
  \ with strict alignment);\n    no DNSSEC and no CAA.\nnotes:\n- 'Mutual TLS on the Business Gateway is the defining control in this estate: businessgateway.landregistry.gov.uk\n  and bgtest.landregistry.gov.uk will not complete a handshake without an HMLR-issued client certificate.'\n- No CAA record on any HMLR registrable domain, and DNSSEC is signed on www.gov.uk but not on landregistry.gov.uk\n  or data.gov.uk.\n- landregistry.data.gov.uk negotiates only TLSv1.2 and sets no HSTS header, the weakest transport posture\n  of the reachable hosts — though it serves nothing but open data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/security/hm-land-registry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- United Kingdom
- Land Registry
- Open Data
- Title
- Conveyancing
- Property Records
- Price Paid Data
- Linked Data
- Geospatial
- Government
- PropTech
---
