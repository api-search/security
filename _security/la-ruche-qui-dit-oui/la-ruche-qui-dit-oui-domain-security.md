---
api_specs:
- filename: la-ruche-qui-dit-oui-api-openapi.yml
  format: yaml
  label: The Food Assembly API
  slug: food-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-ruche-qui-dit-oui/refs/heads/main/openapi/la-ruche-qui-dit-oui-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: laruchequiditoui.fr
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thefoodassembly.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: laruchequiditoui.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.thefoodassembly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Ruche Qui Dit Oui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Ruche qui dit Oui!, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: La Ruche qui dit Oui!
provider_slug: la-ruche-qui-dit-oui
slug: la-ruche-qui-dit-oui-domain-security
source_filename: la-ruche-qui-dit-oui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laruchequiditoui.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\n- host: api.thefoodassembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: laruchequiditoui.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thefoodassembly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-ruche-qui-dit-oui/refs/heads/main/security/la-ruche-qui-dit-oui-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Agriculture
- Marketplace
- E-Commerce
- Local Food
- Sustainability
- France
---
