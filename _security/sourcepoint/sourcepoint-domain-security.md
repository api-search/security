---
api_specs:
- filename: sourcepoint-gdpr-reporting-api-api-openapi.yml
  format: yaml
  label: Sourcepoint GDPR reporting API
  slug: sourcepoint-gdpr-reporting-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-gdpr-reporting-api-api-openapi.yml
- filename: sourcepoint-gdpr-standard-end-user-consent-status-api-openapi.yml
  format: yaml
  label: Sourcepoint GDPR Standard end-user consent status API
  slug: sourcepoint-gdpr-standard-end-user-consent-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-gdpr-standard-end-user-consent-status-api-openapi.yml
- filename: sourcepoint-gdpr-standard-vendor-list-api-openapi.yml
  format: yaml
  label: Sourcepoint GDPR Standard vendor list API
  slug: sourcepoint-gdpr-standard-vendor-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-gdpr-standard-vendor-list-api-openapi.yml
- filename: sourcepoint-gdpr-tcf-end-user-consent-status-api-openapi.yml
  format: yaml
  label: Sourcepoint GDPR TCF end-user consent status API
  slug: sourcepoint-gdpr-tcf-end-user-consent-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-gdpr-tcf-end-user-consent-status-api-openapi.yml
- filename: sourcepoint-gdpr-tcf-vendor-list-api-openapi.yml
  format: yaml
  label: Sourcepoint GDPR TCF vendor list API
  slug: sourcepoint-gdpr-tcf-vendor-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-gdpr-tcf-vendor-list-api-openapi.yml
- filename: sourcepoint-global-enterprise-end-user-consent-status-api-openapi.yml
  format: yaml
  label: Sourcepoint Global Enterprise end-user consent status API
  slug: sourcepoint-global-enterprise-end-user-consent-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-global-enterprise-end-user-consent-status-api-openapi.yml
- filename: sourcepoint-preferences-end-user-history-api-openapi.yml
  format: yaml
  label: Sourcepoint Preferences end-user history API
  slug: sourcepoint-preferences-end-user-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-preferences-end-user-history-api-openapi.yml
- filename: sourcepoint-u-s-multi-state-privacy-end-user-consent-status-api-openapi.yml
  format: yaml
  label: Sourcepoint U.S. Multi-State Privacy end-user consent status API
  slug: sourcepoint-u-s-multi-state-privacy-end-user-consent-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-u-s-multi-state-privacy-end-user-consent-status-api-openapi.yml
- filename: sourcepoint-u-s-multi-state-privacy-reporting-api-api-openapi.yml
  format: yaml
  label: Sourcepoint U.S. Multi-State Privacy reporting API
  slug: sourcepoint-u-s-multi-state-privacy-reporting-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/openapi/sourcepoint-u-s-multi-state-privacy-reporting-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sourcepoint.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: privacy-mgmt.com
  note: The CMP delivery domain that serves the consent APIs and the web wrapper. No SPF, no DMARC, no CAA and no DS record - it is a service domain, not a mail domain, but the missing CAA leaves certificate issuance unconstrained on the host that fronts every consent call.
  spf: false
hosts:
- cert_expires: Sep 24 06:18:31 2026 GMT
  host: www.sourcepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:43:29 2026 GMT
  host: docs.sourcepoint.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: sourcepoint-public-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: cdn.privacy-mgmt.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: 'Production consent API host (OpenAPI servers[]). HSTS observed on an API response: max-age=15552000; includeSubDomains. Added by the enrichment pass because probe-domain-security.py caps at the first three hosts.'
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: portal.sourcepoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: 'Production reporting API + portal host. HSTS on an API response: max-age=63072000; includeSubDomains; preload. Added by the enrichment pass.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcepoint, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sourcepoint
provider_slug: sourcepoint
slug: sourcepoint-domain-security
source_filename: sourcepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourcepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:18:31 2026 GMT\n  hsts: false\n- host: docs.sourcepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: sourcepoint-public-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdn.privacy-mgmt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: 'Production consent API host (OpenAPI servers[]). HSTS observed on an API response: max-age=15552000;\n    includeSubDomains. Added by the enrichment pass because probe-domain-security.py caps at the first\n    three hosts.'\n- host: portal.sourcepoint.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: 'Production reporting API + portal host. HSTS on an API response: max-age=63072000; includeSubDomains;\n    preload. Added by the enrichment pass.'\ndomains:\n- domain: sourcepoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: privacy-mgmt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  note: The CMP delivery domain that serves the consent APIs and the web wrapper. No SPF, no DMARC, no\n    CAA and no DS record - it is a service domain, not a mail domain, but the missing CAA leaves certificate\n    issuance unconstrained on the host that fronts every consent call.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/security/sourcepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Privacy
- Consent Management
- Consent Management Platform
- CMP
- GDPR
- CCPA
- LGPD
- IAB TCF
- IAB GPP
- USNAT
- DSAR
- Adblock Recovery
- Compliance Monitoring
- Publisher Technology
- AdTech
- MarTech
- Privacy Engineering
- CTV
- OTT
- Mobile SDK
- Web SDK
---
