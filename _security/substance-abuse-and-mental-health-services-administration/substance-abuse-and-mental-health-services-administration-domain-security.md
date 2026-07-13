---
api_specs:
- filename: samhsa-treatment-locator-openapi.yml
  format: yaml
  label: SAMHSA Behavioral Health Treatment Services Locator API
  slug: samhsa-treatment-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/substance-abuse-and-mental-health-services-administration/refs/heads/main/openapi/samhsa-treatment-locator-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "identrust.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: samhsa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: findtreatment.gov
  spf: true
hosts:
- cert_expires: Mar 12 13:51:16 2027 GMT
  host: www.samhsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 11 18:09:31 2027 GMT
  host: findtreatment.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 19:36:01 2026 GMT
  host: www.datafiles.samhsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Substance Abuse And Mental Health Services Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Substance Abuse and Mental Health Services Administration, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Substance Abuse and Mental Health Services Administration
provider_slug: substance-abuse-and-mental-health-services-administration
slug: substance-abuse-and-mental-health-services-administration-domain-security
source_filename: substance-abuse-and-mental-health-services-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.samhsa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 12 13:51:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: findtreatment.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 18:09:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.datafiles.samhsa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 19:36:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: samhsa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: findtreatment.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/substance-abuse-and-mental-health-services-administration/refs/heads/main/security/substance-abuse-and-mental-health-services-administration-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Public Health
- Behavioral Health
- Substance Use Disorders
- Mental Health
- Open Data
- Healthcare
---
