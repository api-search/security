---
api_specs:
- filename: amazon-workspaces-web-browsersettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web BrowserSettings API
  slug: amazon-workspaces-web-browsersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-browsersettings-api-openapi.yml
- filename: amazon-workspaces-web-identityproviders-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web IdentityProviders API
  slug: amazon-workspaces-web-identityproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-identityproviders-api-openapi.yml
- filename: amazon-workspaces-web-ipaccesssettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web IpAccessSettings API
  slug: amazon-workspaces-web-ipaccesssettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-ipaccesssettings-api-openapi.yml
- filename: amazon-workspaces-web-networksettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web NetworkSettings API
  slug: amazon-workspaces-web-networksettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-networksettings-api-openapi.yml
- filename: amazon-workspaces-web-portalidp-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web PortalIdp API
  slug: amazon-workspaces-web-portalidp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-portalidp-api-openapi.yml
- filename: amazon-workspaces-web-portals-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Portals API
  slug: amazon-workspaces-web-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-portals-api-openapi.yml
- filename: amazon-workspaces-web-tags-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Tags API
  slug: amazon-workspaces-web-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-tags-api-openapi.yml
- filename: amazon-workspaces-web-truststores-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web TrustStores API
  slug: amazon-workspaces-web-truststores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-truststores-api-openapi.yml
- filename: amazon-workspaces-web-useraccessloggingsettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web UserAccessLoggingSettings API
  slug: amazon-workspaces-web-useraccessloggingsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-useraccessloggingsettings-api-openapi.yml
- filename: amazon-workspaces-web-usersettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web UserSettings API
  slug: amazon-workspaces-web-usersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-usersettings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: workspaces-web.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Workspaces Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon WorkSpaces Web, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
slug: amazon-workspaces-web-domain-security
source_filename: amazon-workspaces-web-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: workspaces-web.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/security/amazon-workspaces-web-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
---
