---
api_specs:
- filename: carnegie-mellon-university-delphi-epidata-openapi.yml
  format: yaml
  label: Delphi Epidata API
  slug: delphi-epidata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-delphi-epidata-openapi.yml
- filename: carnegie-mellon-university-cert-vulnerability-notes-openapi.yml
  format: yaml
  label: CERT/CC Vulnerability Notes API
  slug: cert-vulnerability-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-cert-vulnerability-notes-openapi.yml
- filename: carnegie-mellon-university-library-publishing-openapi.yml
  format: yaml
  label: CMU Library Publishing Service API + OAI-PMH
  slug: library-publishing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-library-publishing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cmu.edu
  spf: true
- caa:
  - 0 issue "emsign.com"
  - 0 issuewild "emsign.com"
  - 0 iodef "mailto:caa-reports@sei.cmu.edu"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cert.org
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.cmu.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: api.delphi.cmu.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.kb.cert.org
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carnegie Mellon University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnegie Mellon University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
slug: carnegie-mellon-university-domain-security
source_filename: carnegie-mellon-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.delphi.cmu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: null\n- host: www.kb.cert.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: cmu.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cert.org\n  dnssec: false\n  caa:\n  - 0 issue \"emsign.com\"\n  - 0 issuewild \"emsign.com\"\n  - 0 iodef \"mailto:caa-reports@sei.cmu.edu\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/security/carnegie-mellon-university-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- United States
- Private Research University
- Research
- Epidemiology
- Public Health
- Cybersecurity
- Vulnerability Disclosure
- Scholarly Publishing
- Institutional Repository
- Identity Federation
- Open Access
- Open Data
---
