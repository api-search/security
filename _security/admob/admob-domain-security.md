---
api_specs:
- filename: admob-accounts-api-openapi.yml
  format: yaml
  label: AdMob Accounts API
  slug: admob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-accounts-api-openapi.yml
- filename: admob-adapters-api-openapi.yml
  format: yaml
  label: AdMob Adapters API
  slug: admob-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adapters-api-openapi.yml
- filename: admob-adsources-api-openapi.yml
  format: yaml
  label: AdMob Ad Sources API
  slug: admob-adsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adsources-api-openapi.yml
- filename: admob-adunitmappings-api-openapi.yml
  format: yaml
  label: AdMob Ad Unit Mappings API
  slug: admob-adunitmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adunitmappings-api-openapi.yml
- filename: admob-adunits-api-openapi.yml
  format: yaml
  label: AdMob Ad Units API
  slug: admob-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adunits-api-openapi.yml
- filename: admob-apps-api-openapi.yml
  format: yaml
  label: AdMob Apps API
  slug: admob-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-apps-api-openapi.yml
- filename: admob-campaignreport-api-openapi.yml
  format: yaml
  label: AdMob Campaign Report API
  slug: admob-campaignreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-campaignreport-api-openapi.yml
- filename: admob-mediationabexperiments-api-openapi.yml
  format: yaml
  label: AdMob Mediation Ab Experiments API
  slug: admob-mediationabexperiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationabexperiments-api-openapi.yml
- filename: admob-mediationgroups-api-openapi.yml
  format: yaml
  label: AdMob Mediation Groups API
  slug: admob-mediationgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationgroups-api-openapi.yml
- filename: admob-mediationreport-api-openapi.yml
  format: yaml
  label: AdMob Mediation Report API
  slug: admob-mediationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationreport-api-openapi.yml
- filename: admob-networkreport-api-openapi.yml
  format: yaml
  label: AdMob Network Report API
  slug: admob-networkreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-networkreport-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: admob.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: admob.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Admob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdMob, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AdMob
provider_slug: admob
slug: admob-domain-security
source_filename: admob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: admob.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: admob.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/security/admob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Mobile
- Monetization
- Ads
- Google
- Reporting
- Mediation
- AdTech
---
