---
api_specs:
- filename: valimail-accounts-api-openapi.yml
  format: yaml
  label: Valimail Accounts API
  slug: valimail-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-accounts-api-openapi.yml
- filename: valimail-authentication-api-openapi.yml
  format: yaml
  label: Valimail Authentication API
  slug: valimail-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-authentication-api-openapi.yml
- filename: valimail-dkims-by-domain-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Domain API
  slug: valimail-dkims-by-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-domain-api-openapi.yml
- filename: valimail-dkims-by-sender-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Sender API
  slug: valimail-dkims-by-sender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-sender-api-openapi.yml
- filename: valimail-domains-api-openapi.yml
  format: yaml
  label: Valimail Domains API
  slug: valimail-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-domains-api-openapi.yml
- filename: valimail-mta-sts-policy-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy API
  slug: valimail-mta-sts-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-api-openapi.yml
- filename: valimail-mta-sts-policy-reports-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy Reports API
  slug: valimail-mta-sts-policy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-reports-api-openapi.yml
- filename: valimail-netblocks-api-openapi.yml
  format: yaml
  label: Valimail Netblocks API
  slug: valimail-netblocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-netblocks-api-openapi.yml
- filename: valimail-portfolios-api-openapi.yml
  format: yaml
  label: Valimail Portfolios API
  slug: valimail-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-portfolios-api-openapi.yml
- filename: valimail-scim-api-openapi.yml
  format: yaml
  label: Valimail SCIM API
  slug: valimail-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-scim-api-openapi.yml
- filename: valimail-senders-api-openapi.yml
  format: yaml
  label: Valimail Senders API
  slug: valimail-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-senders-api-openapi.yml
- filename: valimail-sso-api-openapi.yml
  format: yaml
  label: Valimail SSO API
  slug: valimail-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-sso-api-openapi.yml
- filename: valimail-tls-configuration-api-openapi.yml
  format: yaml
  label: Valimail TLS Configuration API
  slug: valimail-tls-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-tls-configuration-api-openapi.yml
- filename: valimail-users-api-openapi.yml
  format: yaml
  label: Valimail Users API
  slug: valimail-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-users-api-openapi.yml
- filename: valimail-webhooks-api-openapi.yml
  format: yaml
  label: Valimail Webhooks API
  slug: valimail-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-webhooks-api-openapi.yml
- filename: valimail-senders-reports-api-openapi.yml
  format: yaml
  label: Valimail Senders Reports API
  slug: valimail-senders-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-senders-reports-api-openapi.yml
- filename: valimail-teams-api-openapi.yml
  format: yaml
  label: Valimail Teams API
  slug: valimail-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:dmarc_agg@vali.email,mailto:dmarc.reports@valimail.com
  dnssec: false
  domain: valimail.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc_agg@vali.email
  dnssec: false
  domain: valimail-staging.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.valimail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.valimail.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63113904
  hsts_preload: true
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: app.valimail.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 17 13:50:05 2026 GMT
  host: support.valimail.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: Intercom-hosted help center (third-party host, not Valimail infrastructure).
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.valimail-staging.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  note: Stage test server declared in the published Configuration/Account/Partner OpenAPI servers[].
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Valimail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valimail, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Valimail
provider_slug: valimail
slug: valimail-domain-security
source_filename: valimail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI servers[] hosts\nhosts:\n- host: www.valimail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.valimail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: app.valimail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63113904\n- host: support.valimail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:50:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: Intercom-hosted help center (third-party host, not Valimail infrastructure).\n- host: api.valimail-staging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age:\
  \ 63113904\n  note: Stage test server declared in the published Configuration/Account/Partner OpenAPI servers[].\ndomains:\n- domain: valimail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject; rua=mailto:dmarc_agg@vali.email,mailto:dmarc.reports@valimail.com\n- domain: valimail-staging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc_agg@vali.email\nnotes: >-\n  Valimail dogfoods its own product: the corporate domain publishes DMARC at\n  p=reject with aggregate reporting to vali.email. No CAA records and no DNSSEC\n  on either registrable domain (probed 2026-08-14) — both are honest absences.\n  HSTS is set with includeSubDomains + preload on the API host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/security/valimail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Authentication
- DMARC
- Email Security
- SPF
- DKIM
- BIMI
- MTA-STS
- Anti-Phishing
- Deliverability
- Cybersecurity
---
