---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Moosend API
  slug: moosend-api
  spec_type: OpenAPI
  url: https://moosendapp.docs.apiary.io/
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moosend.com
  spf: true
hosts:
- cert_expires: Apr  6 16:03:03 2027 GMT
  host: moosend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 18:02:44 2026 GMT
  host: api.moosend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moosend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moosend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moosend
provider_slug: moosend
slug: moosend-domain-security
source_filename: moosend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moosend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 16:03:03 2027 GMT\n  hsts: false\n- host: api.moosend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:02:44 2026 GMT\n  hsts: null\ndomains:\n- domain: moosend.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/security/moosend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Marketing Automation
- Campaigns
- Mailing Lists
- Subscribers
- Transactional Email
- SMTP
- Segmentation
- Analytics
---
