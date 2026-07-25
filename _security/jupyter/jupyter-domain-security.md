---
api_specs:
- filename: jupyter-config-api-openapi.yml
  format: yaml
  label: Jupyter Config API
  slug: jupyter-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-config-api-openapi.yml
- filename: jupyter-contents-api-openapi.yml
  format: yaml
  label: Jupyter Contents API
  slug: jupyter-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-contents-api-openapi.yml
- filename: jupyter-jupyter-server-rest-api-api-openapi.yml
  format: yaml
  label: Jupyter Jupyter Server REST API API
  slug: jupyter-jupyter-server-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-jupyter-server-rest-api-api-openapi.yml
- filename: jupyter-kernels-api-openapi.yml
  format: yaml
  label: Jupyter Kernels API
  slug: jupyter-kernels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-kernels-api-openapi.yml
- filename: jupyter-kernelspecs-api-openapi.yml
  format: yaml
  label: Jupyter Kernelspecs API
  slug: jupyter-kernelspecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-kernelspecs-api-openapi.yml
- filename: jupyter-me-api-openapi.yml
  format: yaml
  label: Jupyter Me API
  slug: jupyter-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-me-api-openapi.yml
- filename: jupyter-sessions-api-openapi.yml
  format: yaml
  label: Jupyter Sessions API
  slug: jupyter-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-sessions-api-openapi.yml
- filename: jupyter-status-api-openapi.yml
  format: yaml
  label: Jupyter Status API
  slug: jupyter-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-status-api-openapi.yml
- filename: jupyter-terminals-api-openapi.yml
  format: yaml
  label: Jupyter Terminals API
  slug: jupyter-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/openapi/jupyter-terminals-api-openapi.yml
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
  host: jupyter-notebook.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: jupyter-server.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupyter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupyter, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jupyter
provider_slug: jupyter
slug: jupyter-domain-security
source_filename: jupyter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupyter.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:54 2026 GMT\n  hsts: false\n- host: jupyter-notebook.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jupyter-server.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jupyter.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter/refs/heads/main/security/jupyter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Science
- Education
- Interactive Computing
- Notebooks
- Python
- Scientific Computing
---
