---
api_specs:
- filename: liberty-global-applications-api-openapi.yml
  format: yaml
  label: Liberty Global Applications API
  slug: liberty-global-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-applications-api-openapi.yml
- filename: liberty-global-maintainer-api-openapi.yml
  format: yaml
  label: Liberty Global Maintainer API
  slug: liberty-global-maintainer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-maintainer-api-openapi.yml
- filename: liberty-global-stb-api-openapi.yml
  format: yaml
  label: Liberty Global STB API
  slug: liberty-global-stb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-stb-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issuewild "amazontrust.com"
  - 0 iodef "mailto:pki@libertyglobal.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: libertyglobal.com
  spf: true
hosts:
- cert_expires: Mar 27 12:42:18 2027 GMT
  host: www.libertyglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liberty Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liberty Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Liberty Global
provider_slug: liberty-global
slug: liberty-global-domain-security
source_filename: liberty-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.libertyglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 12:42:18 2027 GMT\n  hsts: false\ndomains:\n- domain: libertyglobal.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 iodef \"mailto:pki@libertyglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/security/liberty-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- United Kingdom
- Broadband
- Fixed Broadband
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Europe
- Set-Top Box
- RDK
---
