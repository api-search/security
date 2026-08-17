---
api_specs:
- filename: metrilo-categories-api-openapi.yml
  format: yaml
  label: Metrilo Categories API
  slug: metrilo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-categories-api-openapi.yml
- filename: metrilo-customers-api-openapi.yml
  format: yaml
  label: Metrilo Customers API
  slug: metrilo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-customers-api-openapi.yml
- filename: metrilo-orders-api-openapi.yml
  format: yaml
  label: Metrilo Orders API
  slug: metrilo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-orders-api-openapi.yml
- filename: metrilo-products-api-openapi.yml
  format: yaml
  label: Metrilo Products API
  slug: metrilo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-products-api-openapi.yml
- filename: metrilo-tracking-api-openapi.yml
  format: yaml
  label: Metrilo Tracking API
  slug: metrilo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: mtrl.me
  misconfiguration: A TXT record EXISTS at _dmarc.mtrl.me but its value is an SPF policy ("v=spf1 include:mailgun.org ~all"), not a DMARC policy. Because it does not begin with "v=DMARC1", it provides no DMARC protection at all — the domain is unprotected while appearing to have a record. This is a copy-paste misconfiguration, not an absence.
  role: api
  spf: true
  spf_record: v=spf1 include:mailgun.org ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:rua@dmarc.brevo.com
  dnssec: false
  domain: metrilo.com
  note: DMARC is present but set to p=none (monitor only — no quarantine or reject). Aggregate reports are routed to rua@dmarc.brevo.com, independent DNS-level confirmation that Metrilo mail is administered by Brevo, the 2021 acquirer.
  role: website / mail
  spf: true
  spf_record: v=spf1 a mx include:spf.mail.intercom.io include:mailgun.org include:_spf.google.com ~all
hosts:
- cert_expires: Nov  7 00:58:21 2026 GMT
  cert_valid: true
  host: trk.mtrl.me
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: HSTS is served on the API host but max-age is 15724800s (182 days) — under the 31536000s (1 year) required for HSTS preload eligibility. An unauthenticated POST to /v2/customer returns 401 (endpoint live); GET returns 405. Fronted by Cloudflare.
  role: api ingestion
  tls_version: TLSv1.3
- cert_valid: true
  host: www.metrilo.com
  hsts: false
  https: true
  note: No HSTS on the marketing site. Also answers HTTP 200 with the same marketing HTML to arbitrary paths including every /.well-known/* probe — see well-known/metrilo-well-known.yml.
  role: website
  tls_version: TLSv1.3
- cert_valid: true
  host: app.metrilo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  role: application / login
  tls_version: TLSv1.3
- cert_valid: true
  host: docs.metrilo.com
  hsts: false
  https: true
  role: documentation (Intercom-hosted help center)
  third_party: Intercom
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metrilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metrilo, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Metrilo
provider_slug: metrilo
slug: metrilo-domain-security
source_filename: metrilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py (which resolves the\n  apis.yml baseURL host), then extended by hand with the same kind of live\n  probe against the website, app and docs hosts and both registrable domains.\n  Every value below was observed on 2026-08-13.\nhosts:\n- host: trk.mtrl.me\n  role: api ingestion\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  cert_expires: Nov  7 00:58:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  note: >-\n    HSTS is served on the API host but max-age is 15724800s (182 days) — under\n    the 31536000s (1 year) required for HSTS preload eligibility.\n    An unauthenticated POST to /v2/customer returns 401 (endpoint live);\n    GET returns 405. Fronted by Cloudflare.\n- host: www.metrilo.com\n  role: website\n  https: true\n  tls_version: TLSv1.3\n  cert_valid:\
  \ true\n  hsts: false\n  note: >-\n    No HSTS on the marketing site. Also answers HTTP 200 with the same\n    marketing HTML to arbitrary paths including every /.well-known/* probe —\n    see well-known/metrilo-well-known.yml.\n- host: app.metrilo.com\n  role: application / login\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n- host: docs.metrilo.com\n  role: documentation (Intercom-hosted help center)\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: false\n  third_party: Intercom\ndomains:\n- domain: mtrl.me\n  role: api\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:mailgun.org ~all'\n  dmarc: false\n  dmarc_policy: null\n  misconfiguration: >-\n    A TXT record EXISTS at _dmarc.mtrl.me but its value is an SPF policy\n    (\"v=spf1 include:mailgun.org ~all\"), not a DMARC policy. Because it does not\n    begin with \"v=DMARC1\", it provides no DMARC protection\
  \ at all — the domain\n    is unprotected while appearing to have a record. This is a copy-paste\n    misconfiguration, not an absence.\n- domain: metrilo.com\n  role: website / mail\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 a mx include:spf.mail.intercom.io include:mailgun.org include:_spf.google.com ~all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:rua@dmarc.brevo.com'\n  note: >-\n    DMARC is present but set to p=none (monitor only — no quarantine or\n    reject). Aggregate reports are routed to rua@dmarc.brevo.com, independent\n    DNS-level confirmation that Metrilo mail is administered by Brevo, the\n    2021 acquirer.\nsummary:\n  hosts_probed: 4\n  https_everywhere: true\n  hsts_hosts: 2\n  hsts_preload_eligible: 0\n  dnssec_domains: 0\n  caa_domains: 0\n  dmarc_enforcing_domains: 0\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/security/metrilo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Analytics
- CRM
- Email Marketing
- Customer Retention
- Tracking
- Marketing
---
