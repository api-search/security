---
api_specs:
- filename: jupyterhub-activity-api-openapi.yml
  format: yaml
  label: JupyterHub Activity API
  slug: jupyterhub-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-activity-api-openapi.yml
- filename: jupyterhub-admin-api-openapi.yml
  format: yaml
  label: JupyterHub Admin API
  slug: jupyterhub-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-admin-api-openapi.yml
- filename: jupyterhub-authorizations-api-openapi.yml
  format: yaml
  label: JupyterHub Authorizations API
  slug: jupyterhub-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-authorizations-api-openapi.yml
- filename: jupyterhub-general-api-openapi.yml
  format: yaml
  label: JupyterHub General API
  slug: jupyterhub-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-general-api-openapi.yml
- filename: jupyterhub-groups-api-openapi.yml
  format: yaml
  label: JupyterHub Groups API
  slug: jupyterhub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-groups-api-openapi.yml
- filename: jupyterhub-oauth2-api-openapi.yml
  format: yaml
  label: JupyterHub OAuth2 API
  slug: jupyterhub-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-oauth2-api-openapi.yml
- filename: jupyterhub-proxy-api-openapi.yml
  format: yaml
  label: JupyterHub Proxy API
  slug: jupyterhub-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-proxy-api-openapi.yml
- filename: jupyterhub-servers-api-openapi.yml
  format: yaml
  label: JupyterHub Servers API
  slug: jupyterhub-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-servers-api-openapi.yml
- filename: jupyterhub-services-api-openapi.yml
  format: yaml
  label: JupyterHub Services API
  slug: jupyterhub-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-services-api-openapi.yml
- filename: jupyterhub-tokens-api-openapi.yml
  format: yaml
  label: JupyterHub Tokens API
  slug: jupyterhub-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-tokens-api-openapi.yml
- filename: jupyterhub-users-api-openapi.yml
  format: yaml
  label: JupyterHub Users API
  slug: jupyterhub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jupyter.org
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Sep 19 11:01:54 2026 GMT
  host: jupyter.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: jupyterhub.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupyterhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JupyterHub, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JupyterHub
provider_slug: jupyterhub
slug: jupyterhub-domain-security
source_filename: jupyterhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupyter.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:54 2026 GMT\n  hsts: false\n- host: jupyterhub.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jupyter.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/security/jupyterhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- Python
---
