---
api_specs:
- filename: xcel-energy-green-button-api.yaml
  format: yaml
  label: Xcel Energy Green Button Connect My Data API
  slug: xcel-energy-green-button-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-green-button-api.yaml
- filename: xcel-energy-smart-meter-api.yaml
  format: yaml
  label: Xcel Energy Smart Meter IEEE 2030.5 API
  slug: xcel-energy-smart-meter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-smart-meter-api.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "oaticerts.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xcelenergy.com
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: developer-apim.aws.xcelenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api.xcelenergy.com
  https: false
kind: domain-security
layout: security
method: probed
name: Xcel Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xcel Energy, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xcel Energy
provider_slug: xcel-energy
slug: xcel-energy-domain-security
source_filename: xcel-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-apim.aws.xcelenergy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: null\n- host: api.xcelenergy.com\n  https: false\ndomains:\n- domain: xcelenergy.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"oaticerts.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/security/xcel-energy-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Electric Utility
- Energy
- Energy Data
- Green Button
- Natural Gas
- Smart Grid
- Smart Meter
- Utility
- ESPI
- IEEE 2030.5
- Fortune 500
---
