---
api_specs:
- filename: usercentrics-ccpa-api-openapi.yml
  format: yaml
  label: Usercentrics CCPA API
  slug: usercentrics-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-ccpa-api-openapi.yml
- filename: usercentrics-consent-api-openapi.yml
  format: yaml
  label: Usercentrics Consent API
  slug: usercentrics-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-consent-api-openapi.yml
- filename: usercentrics-consent-mode-api-openapi.yml
  format: yaml
  label: Usercentrics Consent Mode API
  slug: usercentrics-consent-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-consent-mode-api-openapi.yml
- filename: usercentrics-controller-api-openapi.yml
  format: yaml
  label: Usercentrics Controller API
  slug: usercentrics-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-controller-api-openapi.yml
- filename: usercentrics-dialog-api-openapi.yml
  format: yaml
  label: Usercentrics Dialog API
  slug: usercentrics-dialog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-dialog-api-openapi.yml
- filename: usercentrics-gpp-api-openapi.yml
  format: yaml
  label: Usercentrics GPP API
  slug: usercentrics-gpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-gpp-api-openapi.yml
- filename: usercentrics-lifecycle-api-openapi.yml
  format: yaml
  label: Usercentrics Lifecycle API
  slug: usercentrics-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-lifecycle-api-openapi.yml
- filename: usercentrics-scanner-api-openapi.yml
  format: yaml
  label: Usercentrics Scanner API
  slug: usercentrics-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-scanner-api-openapi.yml
- filename: usercentrics-tcf-api-openapi.yml
  format: yaml
  label: Usercentrics TCF API
  slug: usercentrics-tcf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-tcf-api-openapi.yml
- filename: usercentrics-ui-api-openapi.yml
  format: yaml
  label: Usercentrics UI API
  slug: usercentrics-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-ui-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usercentrics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cookiebot.com
  spf: true
hosts:
- cert_expires: Sep 15 05:37:49 2026 GMT
  host: usercentrics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:39:31 2026 GMT
  host: docs.usercentrics.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:05:53 2026 GMT
  host: www.cookiebot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usercentrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usercentrics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Usercentrics
provider_slug: usercentrics
slug: usercentrics-domain-security
source_filename: usercentrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usercentrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.usercentrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:39:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: www.cookiebot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:05:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usercentrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cookiebot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/security/usercentrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Privacy
- Consent
- CMP
- Compliance
- GDPR
- CCPA
- TCF
- GPP
- Cookies
- AI Governance
---
