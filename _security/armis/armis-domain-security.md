---
api_specs:
- filename: armis-alerts-api-openapi.yml
  format: yaml
  label: Armis Alerts API
  slug: armis-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-alerts-api-openapi.yml
- filename: armis-arp-api-openapi.yml
  format: yaml
  label: Armis ARP API
  slug: armis-arp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-arp-api-openapi.yml
- filename: armis-assets-api-openapi.yml
  format: yaml
  label: Armis Assets API
  slug: armis-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-assets-api-openapi.yml
- filename: armis-authentication-api-openapi.yml
  format: yaml
  label: Armis Authentication API
  slug: armis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-authentication-api-openapi.yml
- filename: armis-boundaries-api-openapi.yml
  format: yaml
  label: Armis Boundaries API
  slug: armis-boundaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-boundaries-api-openapi.yml
- filename: armis-collectors-api-openapi.yml
  format: yaml
  label: Armis Collectors API
  slug: armis-collectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-collectors-api-openapi.yml
- filename: armis-data-export-api-openapi.yml
  format: yaml
  label: Armis Data Export API
  slug: armis-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-data-export-api-openapi.yml
- filename: armis-device-custom-properties-api-openapi.yml
  format: yaml
  label: Armis Device Custom Properties API
  slug: armis-device-custom-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-device-custom-properties-api-openapi.yml
- filename: armis-integrations-api-openapi.yml
  format: yaml
  label: Armis Integrations API
  slug: armis-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-integrations-api-openapi.yml
- filename: armis-policies-api-openapi.yml
  format: yaml
  label: Armis Policies API
  slug: armis-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-policies-api-openapi.yml
- filename: armis-sites-api-openapi.yml
  format: yaml
  label: Armis Sites API
  slug: armis-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-sites-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: armis.com
  spf: true
hosts:
- cert_expires: Jan  1 18:02:58 2027 GMT
  host: www.armis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Armis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Armis
provider_slug: armis
slug: armis-domain-security
source_filename: armis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 18:02:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: armis.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/security/armis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense Government
- Security
- Cybersecurity
- Asset Intelligence
- Exposure Management
- IoT
- OT Security
- Vulnerability Management
- Developer Tools
---
