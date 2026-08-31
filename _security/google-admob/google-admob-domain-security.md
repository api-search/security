---
api_specs:
- filename: google-admob-accounts-api-openapi.yml
  format: yaml
  label: Google AdMob Accounts API
  slug: google-admob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-accounts-api-openapi.yml
- filename: google-admob-adapters-api-openapi.yml
  format: yaml
  label: Google AdMob Adapters API
  slug: google-admob-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adapters-api-openapi.yml
- filename: google-admob-adsources-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Sources API
  slug: google-admob-adsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adsources-api-openapi.yml
- filename: google-admob-adunitmappings-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Unit Mappings API
  slug: google-admob-adunitmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adunitmappings-api-openapi.yml
- filename: google-admob-adunits-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Units API
  slug: google-admob-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adunits-api-openapi.yml
- filename: google-admob-apps-api-openapi.yml
  format: yaml
  label: Google AdMob Apps API
  slug: google-admob-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-apps-api-openapi.yml
- filename: google-admob-campaignreport-api-openapi.yml
  format: yaml
  label: Google AdMob Campaign Report API
  slug: google-admob-campaignreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-campaignreport-api-openapi.yml
- filename: google-admob-mediationabexperiments-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Ab Experiments API
  slug: google-admob-mediationabexperiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationabexperiments-api-openapi.yml
- filename: google-admob-mediationgroups-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Groups API
  slug: google-admob-mediationgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationgroups-api-openapi.yml
- filename: google-admob-mediationreport-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Report API
  slug: google-admob-mediationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationreport-api-openapi.yml
- filename: google-admob-networkreport-api-openapi.yml
  format: yaml
  label: Google AdMob Network Report API
  slug: google-admob-networkreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-networkreport-api-openapi.yml
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
name: Google Admob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google AdMob, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google AdMob
provider_slug: google-admob
slug: google-admob-domain-security
source_filename: google-admob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: admob.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/security/google-admob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ad Mediation
- AdMob
- Advertising
- App Monetization
- Mobile Advertising
- Mobile Apps
- Reports
- Reporting
---
