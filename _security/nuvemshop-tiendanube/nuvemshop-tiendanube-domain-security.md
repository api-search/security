---
api_specs:
- filename: nuvemshop-tiendanube-events-asyncapi.yml
  format: yaml
  label: Nuvemshop Tiendanube API
  slug: nuvemshop-tiendanube-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/asyncapi/nuvemshop-tiendanube-events-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuvemshop.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tiendanube.com
  spf: true
hosts:
- cert_expires: Aug 24 18:30:15 2026 GMT
  host: www.nuvemshop.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 08:15:08 2026 GMT
  host: api.tiendanube.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuvemshop Tiendanube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvemshop Tiendanube, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuvemshop Tiendanube
provider_slug: nuvemshop-tiendanube
slug: nuvemshop-tiendanube-domain-security
source_filename: nuvemshop-tiendanube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nuvemshop.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:30:15 2026 GMT\n  hsts: false\n- host: api.tiendanube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:15:08 2026 GMT\n  hsts: null\ndomains:\n- domain: nuvemshop.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tiendanube.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/security/nuvemshop-tiendanube-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Retail
- Online Stores
- Payments
- Shipping
- Webhooks
- OAuth
- Latin America
- Storefront
- Apps Platform
---
