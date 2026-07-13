---
api_specs:
- filename: university-of-sheffield-orda.yaml
  format: yaml
  label: ORDA Research Data Repository (figshare API)
  slug: orda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-orda.yaml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:soc@sheffield.ac.uk"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sheffield.ac.uk
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:soc@sheffield.ac.uk"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shef.ac.uk
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.sheffield.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: orda.shef.ac.uk
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
name: University Of Sheffield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Sheffield, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Sheffield
provider_slug: university-of-sheffield
slug: university-of-sheffield-domain-security
source_filename: university-of-sheffield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sheffield.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: orda.shef.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sheffield.ac.uk\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:soc@sheffield.ac.uk\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shef.ac.uk\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild\
  \ \"sectigo.com\"\n  - 0 iodef \"mailto:soc@sheffield.ac.uk\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/security/university-of-sheffield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- OAI-PMH
- United Kingdom
---
