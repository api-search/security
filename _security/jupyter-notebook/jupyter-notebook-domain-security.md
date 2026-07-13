---
api_specs:
- filename: jupyter-notebook-rest-api-openapi.yml
  format: yaml
  label: Jupyter Notebook REST API
  slug: jupyter-notebook-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-notebook-rest-api-openapi.yml
- filename: jupyter-kernel-gateway-api-openapi.yml
  format: yaml
  label: Jupyter Kernel Gateway API
  slug: jupyter-kernel-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyter-kernel-gateway-api-openapi.yml
- filename: jupyterhub-rest-api-openapi.yml
  format: yaml
  label: JupyterHub REST API
  slug: jupyterhub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/openapi/jupyterhub-rest-api-openapi.yml
- filename: jupyter-kernel-messaging-asyncapi.yml
  format: yaml
  label: Jupyter Kernel Messaging Protocol
  slug: jupyter-kernel-messaging
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/asyncapi/jupyter-kernel-messaging-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jupyter.org
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
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
  host: jupyter-notebook.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: jupyter-kernel-gateway.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupyter Notebook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupyter Notebook, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jupyter Notebook
provider_slug: jupyter-notebook
slug: jupyter-notebook-domain-security
source_filename: jupyter-notebook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupyter.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:54 2026 GMT\n  hsts: false\n- host: jupyter-notebook.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jupyter-kernel-gateway.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jupyter.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/security/jupyter-notebook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Science
- Interactive Computing
- Jupyter
- Machine Learning
- Notebooks
- Python
---
