---
api_specs:
- filename: alectra-utilities-applicationinformation-api-openapi.yml
  format: yaml
  label: Alectra Utilities Application Information API
  slug: alectra-utilities-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-applicationinformation-api-openapi.yml
- filename: alectra-utilities-authorization-api-openapi.yml
  format: yaml
  label: Alectra Utilities Authorization API
  slug: alectra-utilities-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-authorization-api-openapi.yml
- filename: alectra-utilities-batch-api-openapi.yml
  format: yaml
  label: Alectra Utilities Batch API
  slug: alectra-utilities-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-batch-api-openapi.yml
- filename: alectra-utilities-usagepoint-api-openapi.yml
  format: yaml
  label: Alectra Utilities Usage Point API
  slug: alectra-utilities-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-usagepoint-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alectrautilities.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenbuttonalliance.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savagedata.com
  note: 'The data custodian vendor domain that actually hosts every Alectra Green Button surface. Weaker posture than Alectra''s own domain on all three counts: no DNSSEC (Alectra has it), no CAA records (Alectra pins Sectigo and Let''s Encrypt), and DMARC p=quarantine rather than Alectra''s p=reject. HSTS max-age on the three vendor hosts is 2592000 (30 days) against 31622400 (366 days) on alectrautilities.com. Recorded because the regulated data surface lives here, not on the domain whose posture Alectra controls.'
  spf: true
  spf_record: v=spf1 mx ip4:206.47.119.162 -all
hosts:
- cert_expires: Sep  1 11:55:24 2026 GMT
  host: alectrautilities.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: myalectra.alectrautilities.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 20:26:53 2026 GMT
  host: sandbox.greenbuttonalliance.org
  hsts: null
  https: true
  note: Not an Alectra host. This is the Green Button Alliance public sandbox declared in the servers[] block of the harvested standard specification.
  tls_version: TLSv1.3
- cert_expires: Nov 17 14:06:38 2026 GMT
  host: alectrautilitiesgbportal.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Alectra-branded Green Button customer portal / Data Custodian front end, operated by the vendor Savage Data Systems on savagedata.com rather than on an Alectra domain. Probed manually and added to this file — the pipeline host collector only walks apis.yml Website/Portal/humanURL/baseURL and OpenAPI servers[].
  tls_version: TLSv1.3
- cert_expires: Nov 17 14:06:38 2026 GMT
  host: alectrautilitiesonboarding.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Alectra third-party registration and onboarding application, vendor-hosted.
  tls_version: TLSv1.3
- cert_expires: Nov 17 14:06:38 2026 GMT
  host: alectrautilitiesdataview.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Commercial and industrial interval-data portal (CSV download), vendor-hosted.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alectra Utilities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alectra Utilities, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alectra Utilities
provider_slug: alectra-utilities
slug: alectra-utilities-domain-security
source_filename: alectra-utilities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alectrautilities.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:55:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: myalectra.alectrautilities.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:26:53 2026 GMT\n  hsts: null\n  note: >-\n    Not an Alectra host. This is the Green Button Alliance public sandbox declared in\n    the servers[] block of the harvested standard specification.\n- host: alectrautilitiesgbportal.savagedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: >-\n    Alectra-branded Green Button customer portal / Data Custodian front end, operated\n\
  \    by the vendor Savage Data Systems on savagedata.com rather than on an Alectra\n    domain. Probed manually and added to this file — the pipeline host collector only\n    walks apis.yml Website/Portal/humanURL/baseURL and OpenAPI servers[].\n- host: alectrautilitiesonboarding.savagedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: Alectra third-party registration and onboarding application, vendor-hosted.\n- host: alectrautilitiesdataview.savagedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: Commercial and industrial interval-data portal (CSV download), vendor-hosted.\ndomains:\n- domain: alectrautilities.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n- domain: greenbuttonalliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: savagedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 mx ip4:206.47.119.162 -all\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    The data custodian vendor domain that actually hosts every Alectra Green Button\n    surface. Weaker posture than Alectra's own domain on all three counts: no DNSSEC\n    (Alectra has it), no CAA records (Alectra pins Sectigo and Let's Encrypt), and\n    DMARC p=quarantine rather than Alectra's p=reject. HSTS max-age on the three\n    vendor hosts is 2592000 (30 days) against 31622400 (366 days) on\n    alectrautilities.com. Recorded because the regulated data surface lives here, not\n    on the domain whose posture Alectra controls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/security/alectra-utilities-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Ontario
- Green Button
- Smart Metering
- Energy Data
- Grid
- Municipal Utility
- ESPI
---
