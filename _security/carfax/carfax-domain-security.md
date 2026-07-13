---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: CARFAX Vehicle Valuation API
  slug: vehicle-valuation-api
  spec_type: OpenAPI
  url: https://apireference.carfax.ca/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carfax.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: carfaxforlenders.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.carfax.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.carfaxforlenders.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.carfaxserviceshops.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carfax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CARFAX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CARFAX
provider_slug: carfax
slug: carfax-domain-security
source_filename: carfax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carfax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: www.carfaxforlenders.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.carfaxserviceshops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: carfax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: carfaxforlenders.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carfax/refs/heads/main/security/carfax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vehicle History
- VIN Lookup
- Automotive
- Used Cars
- Dealer Tools
- Insurance
- Lending
- QuickVIN
- Service History
---
