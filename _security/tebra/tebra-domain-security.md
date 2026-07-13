---
api_specs:
- filename: tebra-clinical-openapi.yml
  format: yaml
  label: Tebra Clinical Data API
  slug: tebra-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-clinical-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:netops-team@kareo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tebra.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:netops-team@kareo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kareo.com
  spf: true
hosts:
- cert_expires: Aug 31 01:26:34 2026 GMT
  host: www.tebra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: helpme.tebra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: webservice.kareo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tebra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tebra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tebra
provider_slug: tebra
slug: tebra-domain-security
source_filename: tebra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:26:34 2026 GMT\n  hsts: false\n- host: helpme.tebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webservice.kareo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tebra.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:netops-team@kareo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kareo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:netops-team@kareo.com\"\
  \n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/security/tebra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Practice Management
- EHR
- Medical Billing
- Patient Engagement
- Kareo
- PatientPop
---
