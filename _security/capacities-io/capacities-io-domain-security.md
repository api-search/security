---
api_specs:
- filename: capacities-io-blocks-api-openapi.yml
  format: yaml
  label: Capacities Blocks API
  slug: capacities-io-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-blocks-api-openapi.yml
- filename: capacities-io-object-api-openapi.yml
  format: yaml
  label: Capacities Object API
  slug: capacities-io-object-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-object-api-openapi.yml
- filename: capacities-io-objects-api-openapi.yml
  format: yaml
  label: Capacities Objects API
  slug: capacities-io-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-objects-api-openapi.yml
- filename: capacities-io-space-api-openapi.yml
  format: yaml
  label: Capacities Space API
  slug: capacities-io-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-space-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: capacities.io
  spf: true
hosts:
- cert_expires: Dec  9 20:01:51 2026 GMT
  host: capacities.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capacities Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capacities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Capacities
provider_slug: capacities-io
slug: capacities-io-domain-security
source_filename: capacities-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capacities.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 20:01:51 2026 GMT\n  hsts: false\ndomains:\n- domain: capacities.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/capacities-io/security/capacities-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Knowledge Management
- Note Taking
- Productivity
- Cross-Platform
- Collaboration
---
