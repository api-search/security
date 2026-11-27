---
api_specs:
- filename: temoinpublic-fr-dater-api-openapi.yml
  format: yaml
  label: Témoin public Dater API
  slug: temoinpublic-fr-dater-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-dater-api-openapi.yml
- filename: temoinpublic-fr-lire-api-openapi.yml
  format: yaml
  label: Témoin public Lire API
  slug: temoinpublic-fr-lire-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-lire-api-openapi.yml
- filename: temoinpublic-fr-registre-api-openapi.yml
  format: yaml
  label: Témoin public Registre API
  slug: temoinpublic-fr-registre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-registre-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: temoinpublic.fr
  spf: true
hosts:
- cert_expires: Jan 10 18:58:23 2027 GMT
  host: temoinpublic.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Témoin public Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Témoin public, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Témoin public
provider_slug: temoinpublic-fr
slug: temoinpublic-fr-domain-security
source_filename: temoinpublic-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temoinpublic.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 18:58:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: temoinpublic.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/temoinpublic-fr/security/temoinpublic-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
