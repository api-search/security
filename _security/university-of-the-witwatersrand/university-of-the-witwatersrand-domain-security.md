---
api_specs:
- filename: university-of-the-witwatersrand-wiredspace-rest.yaml
  format: yaml
  label: WIReDSpace DSpace REST API
  slug: wiredspace-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-wiredspace-rest.yaml
- filename: university-of-the-witwatersrand-wiredspace-oai.yaml
  format: yaml
  label: WIReDSpace OAI-PMH
  slug: wiredspace-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-wiredspace-oai.yaml
- filename: university-of-the-witwatersrand-open-data-vault.yaml
  format: yaml
  label: Wits Open Data Vault (Figshare)
  slug: open-data-vault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-open-data-vault.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wits.ac.za
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.wits.ac.za
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 11 23:59:59 2026 GMT
  host: wiredspace.wits.ac.za
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 29 21:53:30 2026 GMT
  host: info.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of The Witwatersrand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of the Witwatersrand, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of the Witwatersrand
provider_slug: university-of-the-witwatersrand
slug: university-of-the-witwatersrand-domain-security
source_filename: university-of-the-witwatersrand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wits.ac.za\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: wiredspace.wits.ac.za\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 11 23:59:59 2026 GMT\n  hsts: false\n- host: info.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:53:30 2026 GMT\n  hsts: false\ndomains:\n- domain: wits.ac.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/security/university-of-the-witwatersrand-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Institutional Repository
- South Africa
- Africa
---
