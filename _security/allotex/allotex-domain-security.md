---
api_specs:
- filename: allotex-content-api-openapi.yml
  format: yaml
  label: Allotex Content API
  slug: allotex-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-content-api-openapi.yml
- filename: allotex-discovery-api-openapi.yml
  format: yaml
  label: Allotex Discovery API
  slug: allotex-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-discovery-api-openapi.yml
- filename: allotex-identity-api-openapi.yml
  format: yaml
  label: Allotex Identity API
  slug: allotex-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-identity-api-openapi.yml
- filename: allotex-media-api-openapi.yml
  format: yaml
  label: Allotex Media API
  slug: allotex-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-media-api-openapi.yml
- filename: allotex-schema-api-openapi.yml
  format: yaml
  label: Allotex Schema API
  slug: allotex-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-schema-api-openapi.yml
- filename: allotex-taxonomy-api-openapi.yml
  format: yaml
  label: Allotex Taxonomy API
  slug: allotex-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/openapi/allotex-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allotex.com
  spf: true
hosts:
- cert_expires: Oct 22 21:19:24 2026 GMT
  host: us.allotex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 21:19:24 2026 GMT
  host: allotex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allotex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allotex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allotex
provider_slug: allotex
slug: allotex-domain-security
source_filename: allotex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Scoped to hosts Allotex controls. The mechanical probe also resolved developer.wordpress.org /\n  wordpress.org because the Content API humanURL points at the upstream WordPress REST handbook;\n  those are not Allotex infrastructure and have been removed. Both Allotex hosts are the same\n  WordPress multisite install, served from Kinsta behind Cloudflare (observed response headers:\n  server: cloudflare, ki-edge, x-kinsta-cache).\nhosts:\n- host: us.allotex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:19:24 2026 GMT\n  hsts: false\n- host: allotex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:19:24 2026 GMT\n  hsts: false\ndomains:\n- domain: allotex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- id: no-hsts\n  severity: low\n  detail: >-\n    Neither us.allotex.com\
  \ nor allotex.com returns a Strict-Transport-Security header, so a first\n    request over http is not protected against downgrade.\n- id: no-caa\n  severity: informational\n  detail: >-\n    allotex.com publishes no CAA record, so any public CA may issue for the domain.\n- id: no-dnssec\n  severity: informational\n  detail: allotex.com is not DNSSEC-signed.\n- id: dmarc-policy-none\n  severity: low\n  detail: >-\n    allotex.com publishes SPF and a DMARC record, but the DMARC policy is p=none - failures are\n    reported, not rejected or quarantined.\n- id: x-content-type-options-present\n  severity: informational\n  detail: >-\n    The REST API responses do carry x-content-type-options: nosniff and x-robots-tag: noindex.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allotex/refs/heads/main/security/allotex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- medical-devices
- ophthalmology
- biologics
- vision-correction
- corneal-allograft
- presbyopia
- hyperopia
- refractive-surgery
- tissue-processing
- life-sciences
- clinical-trials
- content-api
---
