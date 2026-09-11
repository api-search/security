---
api_specs:
- filename: first-street-enterprise-api-openapi.yml
  format: yaml
  label: First Street Enterprise API
  slug: first-street-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-enterprise-api-openapi.yml
- filename: first-street-graphql-api-openapi.yml
  format: yaml
  label: First Street Graphql API
  slug: first-street-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-graphql-api-openapi.yml
- filename: first-street-maps-api-openapi.yml
  format: yaml
  label: First Street Maps API
  slug: first-street-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-maps-api-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA record — any CA may issue for this domain.
  dmarc: true
  dmarc_alignment: relaxed (adkim=r, aspf=r)
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:tech@firststreet.org; adkim=r; aspf=r
  dnssec: false
  domain: firststreet.org
  spf: true
  spf_qualifier: ~all (softfail)
  spf_record: v=spf1 a include:_spf.google.com include:44226531.spf04.hubspotemail.net include:mail.zendesk.com include:servers.mcsv.net include:amazonses.com ~all
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: firststreet.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 06:29:53 2026 GMT
  host: docs.firststreet.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: GitBook-hosted.
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.firststreet.org
  hsts: false
  hsts_max_age: null
  https: true
  note: The API host is the only First Street host with NO HSTS header. Every other host in this list sets one, several with preload. Given that the documented authentication style puts the API key in a query string, a missing HSTS on the credential-bearing host is the most actionable finding in this file.
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: mcp.firststreet.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: null
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: auth.firststreet.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: SAML SP metadata host.
  tls_version: null
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: app.firststreet.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Enterprise Suite application.
  tls_version: null
- cert_expires: Nov  5 13:37:22 2026 GMT
  host: status.firststreet.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63113904
  hsts_preload: true
  https: true
  note: Better Stack status page.
  tls_version: TLSv1.3
- cert_expires: Oct 19 10:14:03 2026 GMT
  host: security.firststreet.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Vanta trust centre.
  tls_version: null
hosts_probed: 8
kind: domain-security
layout: security
method: probed
name: First Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Street, probed live across 8 host(s) and 1 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 7 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: First Street
provider_slug: first-street
slug: first-street-domain-security
source_filename: first-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host this record knows\nnote: >-\n  Extends the automated probe (0-working/probe-domain-security.py), which only reads hosts\n  named in apis.yml/OpenAPI and therefore missed mcp, auth, app, status and the trust\n  centre. It also recorded spf: false for firststreet.org, which is WRONG — the apex\n  publishes a valid SPF record; the domain carries twelve TXT records and the probe read\n  the wrong one. The corrected value and the record itself are below.\nhosts:\n- host: firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: GitBook-hosted.\n- host: api.firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts:\
  \ false\n  hsts_max_age: null\n  note: >-\n    The API host is the only First Street host with NO HSTS header. Every other host in\n    this list sets one, several with preload. Given that the documented authentication\n    style puts the API key in a query string, a missing HSTS on the credential-bearing\n    host is the most actionable finding in this file.\n- host: mcp.firststreet.org\n  https: true\n  tls_version: null\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n  hsts_include_subdomains: true\n- host: auth.firststreet.org\n  https: true\n  tls_version: null\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: SAML SP metadata host.\n- host: app.firststreet.org\n  https: true\n  tls_version: null\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n  hsts_include_subdomains: true\n  note: Enterprise Suite\
  \ application.\n- host: status.firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 13:37:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_preload: true\n  hsts_include_subdomains: true\n  note: Better Stack status page.\n- host: security.firststreet.org\n  https: true\n  tls_version: null\n  cert_expires: Oct 19 10:14:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Vanta trust centre.\ndomains:\n- domain: firststreet.org\n  dnssec: false\n  caa: []\n  caa_note: No CAA record — any CA may issue for this domain.\n  spf: true\n  spf_record: >-\n    v=spf1 a include:_spf.google.com include:44226531.spf04.hubspotemail.net\n    include:mail.zendesk.com include:servers.mcsv.net include:amazonses.com ~all\n  spf_qualifier: '~all (softfail)'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; rua=mailto:tech@firststreet.org; adkim=r; aspf=r'\n  dmarc_alignment: relaxed (adkim=r,\
  \ aspf=r)\nfindings:\n  - >-\n    api.firststreet.org serves no Strict-Transport-Security header while every other\n    First Street host does — including mcp, app and auth with preload.\n  - >-\n    No DNSSEC and no CAA record on firststreet.org.\n  - >-\n    DMARC is at p=quarantine with relaxed alignment and a softfail SPF, rather than\n    p=reject with strict alignment.\n  - >-\n    The apex TXT set names the vendor estate — Google Workspace SAML, HubSpot, Zendesk,\n    Mailchimp, Amazon SES, Zoom, 1Password, Wiz and Better Stack.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/security/first-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Risk
- Environment
- Modeling
- Geospatial
- Insurance
- Real Estate
- Data
- GraphQL
- Mapping
---
