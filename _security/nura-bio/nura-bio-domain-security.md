---
api_specs:
- filename: nura-bio-directory-api-openapi.yml
  format: yaml
  label: Nura Bio Directory API
  slug: nura-bio-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-directory-api-openapi.yml
- filename: nura-bio-discovery-api-openapi.yml
  format: yaml
  label: Nura Bio Discovery API
  slug: nura-bio-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-discovery-api-openapi.yml
- filename: nura-bio-media-api-openapi.yml
  format: yaml
  label: Nura Bio Media API
  slug: nura-bio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-media-api-openapi.yml
- filename: nura-bio-pages-api-openapi.yml
  format: yaml
  label: Nura Bio Pages API
  slug: nura-bio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-pages-api-openapi.yml
- filename: nura-bio-portfolio-api-openapi.yml
  format: yaml
  label: Nura Bio Portfolio API
  slug: nura-bio-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-portfolio-api-openapi.yml
- filename: nura-bio-posts-api-openapi.yml
  format: yaml
  label: Nura Bio Posts API
  slug: nura-bio-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-posts-api-openapi.yml
- filename: nura-bio-taxonomy-api-openapi.yml
  format: yaml
  label: Nura Bio Taxonomy API
  slug: nura-bio-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nurabio.com
  spf: true
hosts:
- cert_expires: Oct 23 23:34:18 2026 GMT
  host: nurabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nura Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nura Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nura Bio
provider_slug: nura-bio
slug: nura-bio-domain-security
source_filename: nura-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nurabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:34:18 2026 GMT\n  hsts: false\ndomains:\n- domain: nurabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnote: 'Probed 2026-08-26. Only nurabio.com is scored here. The probe script also walked developer.wordpress.org\n  because that is the humanURL of the content API entry (the upstream WordPress REST handbook, since Nura\n  Bio publishes no reference of its own); that result was removed because wordpress.org is not a domain Nura\n  Bio controls and its posture must not be credited or charged to Nura Bio. Findings: TLS 1.3 is served and\n  the certificate is current, SPF and DMARC are both published with a p=reject policy, but HSTS is not set,\n  DNSSEC is not enabled, and no CAA record is published. The site is WordPress on Kinsta behind Cloudflare.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/security/nura-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- neuroscience
- neurodegeneration
- drug-discovery
- life-sciences
- clinical-trials
- rare-disease
- small-molecule-therapeutics
- content-api
---
