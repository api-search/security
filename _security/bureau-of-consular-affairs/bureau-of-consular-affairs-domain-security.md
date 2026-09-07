---
api_specs:
- filename: bureau-of-consular-affairs-datastore-api-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Datastore API
  slug: bureau-of-consular-affairs-datastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-datastore-api-openapi.yml
- filename: bureau-of-consular-affairs-discovery-api-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Discovery API
  slug: bureau-of-consular-affairs-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-discovery-api-openapi.yml
- filename: bureau-of-consular-affairs-write-api-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Write API
  slug: bureau-of-consular-affairs-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-write-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: state.gov
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Nov 15 13:47:13 2026 GMT
  host: travel.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 14:37:44 2026 GMT
  host: cadatacatalog.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services6.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bureau Of Consular Affairs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Consular Affairs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Consular Affairs
provider_slug: bureau-of-consular-affairs
slug: bureau-of-consular-affairs-domain-security
source_filename: bureau-of-consular-affairs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: travel.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:47:13 2026 GMT\n  hsts: null\n- host: cadatacatalog.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 14:37:44 2026 GMT\n  hsts: null\n- host: services6.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: state.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/security/bureau-of-consular-affairs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Passports
- Travel
- Travel Advisories
- Visas
---
