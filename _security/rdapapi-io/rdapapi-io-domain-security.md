---
api_specs:
- filename: rdapapi-io-asn-api-openapi.yml
  format: yaml
  label: rdapapi-io ASN API
  slug: rdapapi-io-asn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-asn-api-openapi.yml
- filename: rdapapi-io-domain-api-openapi.yml
  format: yaml
  label: rdapapi-io Domain API
  slug: rdapapi-io-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-domain-api-openapi.yml
- filename: rdapapi-io-entity-api-openapi.yml
  format: yaml
  label: rdapapi-io Entity API
  slug: rdapapi-io-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-entity-api-openapi.yml
- filename: rdapapi-io-health-api-openapi.yml
  format: yaml
  label: rdapapi-io Health API
  slug: rdapapi-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-health-api-openapi.yml
- filename: rdapapi-io-ip-api-openapi.yml
  format: yaml
  label: rdapapi-io IP API
  slug: rdapapi-io-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-ip-api-openapi.yml
- filename: rdapapi-io-nameserver-api-openapi.yml
  format: yaml
  label: rdapapi-io Nameserver API
  slug: rdapapi-io-nameserver-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-nameserver-api-openapi.yml
- filename: rdapapi-io-tlds-api-openapi.yml
  format: yaml
  label: rdapapi-io TLDs API
  slug: rdapapi-io-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-tlds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rdapapi.io
  spf: true
hosts:
- cert_expires: Jan 13 18:03:00 2027 GMT
  host: rdapapi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rdapapi Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rdapapi-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: rdapapi-io
provider_slug: rdapapi-io
slug: rdapapi-io-domain-security
source_filename: rdapapi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rdapapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 18:03:00 2027 GMT\n  hsts: false\ndomains:\n- domain: rdapapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/rdapapi-io/security/rdapapi-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- RDAP
- Domain
- API
- Whois
---
