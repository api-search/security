---
api_specs:
- filename: ackogeneralinsurance-enterprise-openapi.yml
  format: yaml
  label: ACKO for Enterprise Partnership API
  slug: acko-for-enterprise-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ackogeneralinsurance/refs/heads/main/openapi/ackogeneralinsurance-enterprise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: acko.com
  spf: true
hosts:
- cert_expires: Oct 16 14:00:29 2026 GMT
  host: www.acko.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- host: demand-internet.internal.live.acko.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ackogeneralinsurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACKO General Insurance, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: ACKO General Insurance
provider_slug: ackogeneralinsurance
slug: ackogeneralinsurance-domain-security
source_filename: ackogeneralinsurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: demand-internet.internal.live.acko.com\n  https: false\ndomains:\n- domain: acko.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ackogeneralinsurance/refs/heads/main/security/ackogeneralinsurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Health Insurance
- Travel Insurance
- Claims
- Policy Administration
- Financial Services
- India
- Enterprise
---
