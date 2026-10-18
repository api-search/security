---
api_specs:
- filename: asendia-closeshipment-api-openapi.yml
  format: yaml
  label: Asendia Close Shipment API
  slug: asendia-closeshipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-closeshipment-api-openapi.yml
- filename: asendia-consolidation-api-openapi.yml
  format: yaml
  label: Asendia Consolidation API
  slug: asendia-consolidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-consolidation-api-openapi.yml
- filename: asendia-dpdtracking-api-openapi.yml
  format: yaml
  label: Asendia DPD Tracking API
  slug: asendia-dpdtracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-dpdtracking-api-openapi.yml
- filename: asendia-dws-api-openapi.yml
  format: yaml
  label: Asendia DWS API
  slug: asendia-dws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-dws-api-openapi.yml
- filename: asendia-externalinvoiceimport-api-openapi.yml
  format: yaml
  label: Asendia External Invoice Import API
  slug: asendia-externalinvoiceimport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-externalinvoiceimport-api-openapi.yml
- filename: asendia-fulfillment-api-openapi.yml
  format: yaml
  label: Asendia Fulfillment API
  slug: asendia-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-fulfillment-api-openapi.yml
- filename: asendia-idmailinterface-api-openapi.yml
  format: yaml
  label: Asendia ID Mail Interface API
  slug: asendia-idmailinterface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-idmailinterface-api-openapi.yml
- filename: asendia-npi-api-openapi.yml
  format: yaml
  label: Asendia NPI API
  slug: asendia-npi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-npi-api-openapi.yml
- filename: asendia-parcel-api-openapi.yml
  format: yaml
  label: Asendia Parcel API
  slug: asendia-parcel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-parcel-api-openapi.yml
- filename: asendia-pudolocator-api-openapi.yml
  format: yaml
  label: Asendia Pudo Locator API
  slug: asendia-pudolocator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-pudolocator-api-openapi.yml
- filename: asendia-puttolight-api-openapi.yml
  format: yaml
  label: Asendia Put To Light API
  slug: asendia-puttolight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-puttolight-api-openapi.yml
- filename: asendia-receptaclesorting-api-openapi.yml
  format: yaml
  label: Asendia Receptacle Sorting API
  slug: asendia-receptaclesorting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-receptaclesorting-api-openapi.yml
- filename: asendia-servicenow-api-openapi.yml
  format: yaml
  label: Asendia Service Now API
  slug: asendia-servicenow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-servicenow-api-openapi.yml
- filename: asendia-shippingplatform-api-openapi.yml
  format: yaml
  label: Asendia Shipping Platform API
  slug: asendia-shippingplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-shippingplatform-api-openapi.yml
- filename: asendia-shippingplatformbulk-api-openapi.yml
  format: yaml
  label: Asendia Shipping Platform Bulk API
  slug: asendia-shippingplatformbulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-shippingplatformbulk-api-openapi.yml
- filename: asendia-tracking-api-openapi.yml
  format: yaml
  label: Asendia Tracking API
  slug: asendia-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-tracking-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "rapidssl.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asendia.com
  spf: true
hosts:
- cert_expires: Dec 24 09:35:34 2026 GMT
  host: www.asendia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asendia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asendia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asendia
provider_slug: asendia
slug: asendia-domain-security
source_filename: asendia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asendia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 09:35:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asendia.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/security/asendia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- Parcel
- Cross-border eCommerce
- Tracking
- Postal
---
