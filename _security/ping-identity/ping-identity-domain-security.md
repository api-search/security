---
api_specs:
- filename: ping-identity-configuration-management-api-openapi.yml
  format: yaml
  label: Ping Identity Configuration Management API
  slug: ping-identity-configuration-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-configuration-management-api-openapi.yml
- filename: ping-identity-davinci-admin-apis-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin APIs API
  slug: ping-identity-davinci-admin-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-apis-api-openapi.yml
- filename: ping-identity-davinci-admin-application-flow-policies-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Application Flow Policies API
  slug: ping-identity-davinci-admin-application-flow-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-application-flow-policies-api-openapi.yml
- filename: ping-identity-davinci-admin-applications-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Applications API
  slug: ping-identity-davinci-admin-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-applications-api-openapi.yml
- filename: ping-identity-davinci-admin-connector-instances-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Connector Instances API
  slug: ping-identity-davinci-admin-connector-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-connector-instances-api-openapi.yml
- filename: ping-identity-davinci-admin-connectors-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Connectors API
  slug: ping-identity-davinci-admin-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-connectors-api-openapi.yml
- filename: ping-identity-davinci-admin-flow-versions-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Flow Versions API
  slug: ping-identity-davinci-admin-flow-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-flow-versions-api-openapi.yml
- filename: ping-identity-davinci-admin-flows-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Flows API
  slug: ping-identity-davinci-admin-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-flows-api-openapi.yml
- filename: ping-identity-davinci-admin-variables-api-openapi.yml
  format: yaml
  label: Ping Identity DaVinci Admin Variables API
  slug: ping-identity-davinci-admin-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-davinci-admin-variables-api-openapi.yml
- filename: ping-identity-environment-management-api-openapi.yml
  format: yaml
  label: Ping Identity Environment Management API
  slug: ping-identity-environment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-environment-management-api-openapi.yml
- filename: ping-identity-environments-api-openapi.yml
  format: yaml
  label: Ping Identity Environments API
  slug: ping-identity-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-environments-api-openapi.yml
- filename: ping-identity-flow-policies-api-openapi.yml
  format: yaml
  label: Ping Identity Flow Policies API
  slug: ping-identity-flow-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-flow-policies-api-openapi.yml
- filename: ping-identity-metrics-api-openapi.yml
  format: yaml
  label: Ping Identity Metrics API
  slug: ping-identity-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-metrics-api-openapi.yml
- filename: ping-identity-pingone-davinci-api-openapi.yml
  format: yaml
  label: Ping Identity PingOne DaVinci API
  slug: ping-identity-pingone-davinci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-pingone-davinci-api-openapi.yml
- filename: ping-identity-snapshots-api-openapi.yml
  format: yaml
  label: Ping Identity Snapshots API
  slug: ping-identity-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-snapshots-api-openapi.yml
- filename: ping-identity-total-identities-api-openapi.yml
  format: yaml
  label: Ping Identity Total Identities API
  slug: ping-identity-total-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-total-identities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingidentity.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingone.com
  spf: true
hosts:
- cert_expires: Sep  4 20:14:53 2026 GMT
  host: www.pingidentity.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: apidocs.pingidentity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.pingone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ping Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ping Identity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ping Identity
provider_slug: ping-identity
slug: ping-identity-domain-security
source_filename: ping-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pingidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: apidocs.pingidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.pingone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pingidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pingone.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/security/ping-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Authentication
- Authorization
- SSO
- MFA
---
