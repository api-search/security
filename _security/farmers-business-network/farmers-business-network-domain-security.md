---
api_specs:
- filename: farmers-business-network-openapi.yml
  format: yaml
  label: FBN Direct Inputs Marketplace
  slug: fbn-direct-inputs-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/openapi/farmers-business-network-openapi.yml
- filename: farmers-business-network-openapi.yml
  format: yaml
  label: FBN Analytics and Insights
  slug: fbn-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/openapi/farmers-business-network-openapi.yml
- filename: farmers-business-network-openapi.yml
  format: yaml
  label: FBN Crop Marketing
  slug: fbn-crop-marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/openapi/farmers-business-network-openapi.yml
- filename: farmers-business-network-openapi.yml
  format: yaml
  label: FBN Finance
  slug: fbn-finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/openapi/farmers-business-network-openapi.yml
- filename: farmers-business-network-openapi.yml
  format: yaml
  label: Norm AI Advisor
  slug: norm-ai-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/openapi/farmers-business-network-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fbn.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.fbn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmers Business Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Business Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Farmers Business Network
provider_slug: farmers-business-network
slug: farmers-business-network-domain-security
source_filename: farmers-business-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fbn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fbn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-business-network/refs/heads/main/security/farmers-business-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AgTech
- Agriculture
- Marketplace
- Farm Analytics
- AI Advisor
---
