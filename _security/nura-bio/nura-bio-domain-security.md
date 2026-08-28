---
api_specs:
- filename: nura-bio-content-api-openapi.yml
  format: yaml
  label: Nura Bio Content API
  slug: nura-bio-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-content-api-openapi.yml
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
- Biotechnology
- Pharmaceuticals
- Neuroscience
- Neurodegeneration
- Drug Discovery
- Life Sciences
- Clinical Trials
- Rare Disease
- Small Molecule Therapeutics
- Content
---
