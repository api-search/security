---
api_specs:
- filename: API_catalog.html
  format: yaml
  label: Windchill REST Services
  slug: windchill-rest-services
  spec_type: OpenAPI
  url: https://support.ptc.com/help/windchill_rest_services/r1.6/en/windchill_rest_services/API_catalog.html
- filename: index.html
  format: yaml
  label: Arena PLM REST API
  slug: arena-plm-rest-api
  spec_type: OpenAPI
  url: https://api.arenasolutions.com/v1/swagger-ui/index.html
- filename: ptc-openapi-generated.yml
  format: yaml
  label: PTC API
  slug: ptc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ptc/openapi/_ae-authored/ptc-openapi-generated.yml
description: ''
domains:
- caa:
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  - 128 issuewild "letsencrypt.org"
  - 128 issue "letsencrypt.org"
  - 128 issue "identrust.com"
  - 128 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ptc.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:arena-domains@ptc.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arenasolutions.com
  spf: true
hosts:
- cert_expires: Jun  2 23:59:59 2027 GMT
  host: www.ptc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 09:49:47 2026 GMT
  host: api.arenasolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 20 23:59:59 2027 GMT
  host: cloudreco.vuforia.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: PTC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PTC, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PTC
provider_slug: ptc
slug: ptc-domain-security
source_filename: ptc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ptc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jun  2 23:59:59 2027 GMT\n  hsts: null\n- host: api.arenasolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 09:49:47 2026 GMT\n  hsts: null\n- host: cloudreco.vuforia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ptc.com\n  dnssec: false\n  caa:\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"identrust.com\"\n  - 128 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arenasolutions.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n\
  \  - 0 iodef \"mailto:arena-domains@ptc.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ptc/security/ptc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial IoT
- PLM
- Augmented Reality
- Field Service Management
- Manufacturing
- CAD
- Digital Transformation
- Industrial
---
