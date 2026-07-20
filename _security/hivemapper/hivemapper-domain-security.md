---
api_specs:
- filename: hivemapper-beemaps-openapi.yml
  format: yaml
  label: Bee Maps (Hivemapper) Developer API
  slug: bee-maps-hivemapper-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hivemapper/refs/heads/main/openapi/hivemapper-beemaps-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hivemapper.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: beemaps.com
  spf: true
hosts:
- cert_expires: Oct  1 05:27:20 2026 GMT
  host: hivemapper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 10:33:01 2026 GMT
  host: docs.beemaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 10:33:01 2026 GMT
  host: beemaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hivemapper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hivemapper, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hivemapper
provider_slug: hivemapper
slug: hivemapper-domain-security
source_filename: hivemapper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hivemapper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:27:20 2026 GMT\n  hsts: false\n- host: docs.beemaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:33:01 2026 GMT\n  hsts: false\n- host: beemaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:33:01 2026 GMT\n  hsts: false\ndomains:\n- domain: hivemapper.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: beemaps.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hivemapper/refs/heads/main/security/hivemapper-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Logistics
- Mapping
- Geospatial
- Imagery
- Location
- Street View
- Mobility
- Machine Learning
- Web3
---
