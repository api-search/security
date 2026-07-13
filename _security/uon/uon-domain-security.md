---
api_specs:
- filename: uon-open-research-figshare.yaml
  format: yaml
  label: Open Research Newcastle (Figshare REST API)
  slug: open-research-figshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-open-research-figshare.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: newcastle.edu.au
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Sep 12 07:34:29 2026 GMT
  host: www.newcastle.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: openresearch.newcastle.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Uon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Newcastle Australia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Newcastle Australia
provider_slug: uon
slug: uon-domain-security
source_filename: uon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newcastle.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 07:34:29 2026 GMT\n  hsts: false\n- host: openresearch.newcastle.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newcastle.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/security/uon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Research
- Open Access
- Repository
- OAI-PMH
- Australia
---
