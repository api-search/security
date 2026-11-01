---
api_specs:
- filename: programmes-net-converters-api-openapi.yml
  format: yaml
  label: programmes-net Converters API
  slug: programmes-net-converters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-converters-api-openapi.yml
- filename: programmes-net-cryptography-hashing-api-openapi.yml
  format: yaml
  label: programmes-net Cryptography & Hashing API
  slug: programmes-net-cryptography-hashing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-cryptography-hashing-api-openapi.yml
- filename: programmes-net-encoders-decoders-api-openapi.yml
  format: yaml
  label: programmes-net Encoders & Decoders API
  slug: programmes-net-encoders-decoders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-encoders-decoders-api-openapi.yml
- filename: programmes-net-formatters-validators-api-openapi.yml
  format: yaml
  label: programmes-net Formatters & Validators API
  slug: programmes-net-formatters-validators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-formatters-validators-api-openapi.yml
- filename: programmes-net-text-tools-api-openapi.yml
  format: yaml
  label: programmes-net Text Tools API
  slug: programmes-net-text-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-text-tools-api-openapi.yml
- filename: programmes-net-web-tools-api-openapi.yml
  format: yaml
  label: programmes-net Web Tools API
  slug: programmes-net-web-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/programmes-net/openapi/programmes-net-web-tools-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@setkernel.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: programmes.net
  spf: true
hosts:
- cert_expires: Dec 10 17:46:30 2026 GMT
  host: programmes.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Programmes Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for programmes-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: programmes-net
provider_slug: programmes-net
slug: programmes-net-domain-security
source_filename: programmes-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: programmes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 17:46:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: programmes.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@setkernel.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/programmes-net/security/programmes-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- API
- OpenAPI
- MCP
---
