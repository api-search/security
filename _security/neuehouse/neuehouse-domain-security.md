---
api_specs:
- filename: neuehouse-content-api-openapi.yml
  format: yaml
  label: NeueHouse Content API
  slug: neuehouse-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuehouse/refs/heads/main/openapi/neuehouse-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neuehouse.com
  spf: true
hosts:
- cert_expires: Nov 14 20:42:50 2026 GMT
  host: www.neuehouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_cn: '*.netlify.app'
  cert_issuer_org: Netlify, Inc
  cert_valid_for_host: false
  finding: 'DEFECT — TLS name mismatch. This host serves a real NeueHouse site (HTML title "NeueHouse: Bradbury", 28KB, HTTP 200 when verification is disabled) from Netlify, but presents a *.netlify.app certificate. subjectAltName does not match bradbury.neuehouse.com, so every standards-compliant client fails the handshake: curl returns exit 60 and browsers show a full-page interstitial. The host is reachable ONLY by disabling certificate verification. NeueHouse links to it from its own live content API (location record id 6421), so the broken link is self-referential. Fix is a custom-domain certificate on the Netlify site.'
  host: bradbury.neuehouse.com
  hsts: null
  https: true
  probed: '2026-08-26'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuehouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeueHouse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NeueHouse
provider_slug: neuehouse
slug: neuehouse-domain-security
source_filename: neuehouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neuehouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 20:42:50 2026 GMT\n  hsts: false\n- host: bradbury.neuehouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid_for_host: false\n  cert_cn: '*.netlify.app'\n  cert_issuer_org: Netlify, Inc\n  hsts: null\n  finding: 'DEFECT — TLS name mismatch. This host serves a real NeueHouse site (HTML title \"NeueHouse:\n    Bradbury\", 28KB, HTTP 200 when verification is disabled) from Netlify, but presents a *.netlify.app\n    certificate. subjectAltName does not match bradbury.neuehouse.com, so every standards-compliant client\n    fails the handshake: curl returns exit 60 and browsers show a full-page interstitial. The host is\n    reachable ONLY by disabling certificate verification. NeueHouse links to it from its own live content\n    API (location record id 6421), so the broken\
  \ link is self-referential. Fix is a custom-domain certificate\n    on the Netlify site.'\n  probed: '2026-08-26'\ndomains:\n- domain: neuehouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: 'forgeglobal.com was removed from this probe set: it is a secondary-market share-listing page that\n  seeded this repo, not a host NeueHouse operates. Hosts probed are the ones NeueHouse actually serves.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuehouse/refs/heads/main/security/neuehouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Coworking
- Events
- Content
- WordPress
- Membership
- Real Estate
- Media
- Workspace
---
