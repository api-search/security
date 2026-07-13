---
api_specs:
- filename: openapi.json
  format: json
  label: PubChem PUG REST API
  slug: pubchem-pug-rest-api
  spec_type: OpenAPI
  url: https://pubchem.ncbi.nlm.nih.gov/rest/pug/openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "identrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nih.gov
  spf: true
hosts:
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: pubchem.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pubchem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubChem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PubChem
provider_slug: pubchem
slug: pubchem-domain-security
source_filename: pubchem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pubchem.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"identrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubchem/refs/heads/main/security/pubchem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Chemistry
- Chemical Compounds
- Drug Discovery
- Bioassay
- Life Sciences
- NCBI
- Bioinformatics
---
