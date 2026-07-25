---
api_specs:
- filename: jupyter-notebooks-contents-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Contents API
  slug: jupyter-notebooks-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-contents-api-openapi.yml
- filename: jupyter-notebooks-kernels-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Kernels API
  slug: jupyter-notebooks-kernels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-kernels-api-openapi.yml
- filename: jupyter-notebooks-kernelspecs-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks KernelSpecs API
  slug: jupyter-notebooks-kernelspecs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-kernelspecs-api-openapi.yml
- filename: jupyter-notebooks-sessions-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Sessions API
  slug: jupyter-notebooks-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-sessions-api-openapi.yml
- filename: jupyter-notebooks-terminals-api-openapi.yml
  format: yaml
  label: Jupyter Notebooks Terminals API
  slug: jupyter-notebooks-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/openapi/jupyter-notebooks-terminals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jupyter.org
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
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
  host: jupyter-server.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupyter Notebooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupyter Notebooks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jupyter Notebooks
provider_slug: jupyter-notebooks
slug: jupyter-notebooks-domain-security
source_filename: jupyter-notebooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupyter.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:54 2026 GMT\n  hsts: false\n- host: jupyter-server.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jupyter.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/security/jupyter-notebooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Science
- Interactive Computing
- Jupyter
- Notebooks
- Python
---
