---
api_specs:
- filename: jupyter-hub-groups-api-openapi.yml
  format: yaml
  label: JupyterHub Groups API
  slug: jupyter-hub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-groups-api-openapi.yml
- filename: jupyter-hub-hub-api-openapi.yml
  format: yaml
  label: JupyterHub Hub API
  slug: jupyter-hub-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-hub-api-openapi.yml
- filename: jupyter-hub-services-api-openapi.yml
  format: yaml
  label: JupyterHub Services API
  slug: jupyter-hub-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-services-api-openapi.yml
- filename: jupyter-hub-tokens-api-openapi.yml
  format: yaml
  label: JupyterHub Tokens API
  slug: jupyter-hub-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-tokens-api-openapi.yml
- filename: jupyter-hub-users-api-openapi.yml
  format: yaml
  label: JupyterHub Users API
  slug: jupyter-hub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/openapi/jupyter-hub-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jupyter.org
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
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
- host: your-jupyterhub-domain.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jupyter Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JupyterHub, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JupyterHub
provider_slug: jupyter-hub
slug: jupyter-hub-domain-security
source_filename: jupyter-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupyter.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:54 2026 GMT\n  hsts: false\n- host: jupyterhub.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-jupyterhub-domain.com\n  https: false\ndomains:\n- domain: jupyter.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/security/jupyter-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Science
- Education
- Jupyter
- Multi-User
- Notebooks
---
