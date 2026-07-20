---
api_specs:
- filename: cachet-parking-openapi.yml
  format: yaml
  label: Cachet Parking API
  slug: cachet-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-parking-openapi.yml
- filename: cachet-verify-openapi.yml
  format: yaml
  label: Cachet Verify / Platform API
  slug: cachet-verify-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-verify-openapi.yml
- filename: cachet-partners-openapi.yml
  format: yaml
  label: Cachet Partners API
  slug: cachet-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-partners-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:devs@cachet.me"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cachet.me
  spf: true
hosts:
- cert_expires: Oct 11 23:58:32 2026 GMT
  host: cachet.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: platform-api.cachet.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: dev-platorm-api.cachet.me
  https: false
kind: domain-security
layout: security
method: probed
name: Cachet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cachet, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cachet
provider_slug: cachet
slug: cachet-domain-security
source_filename: cachet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cachet.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:58:32 2026 GMT\n  hsts: false\n- host: platform-api.cachet.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\n- host: dev-platorm-api.cachet.me\n  https: false\ndomains:\n- domain: cachet.me\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devs@cachet.me\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/security/cachet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- InsurTech
- Mobility
- Gig Economy
- Car Sharing
- Embedded Insurance
- Events
---
