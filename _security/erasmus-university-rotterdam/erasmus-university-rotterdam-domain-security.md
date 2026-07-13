---
api_specs:
- filename: erasmus-university-rotterdam-figshare-data.yaml
  format: yaml
  label: EUR Research Data Repository (Figshare API)
  slug: figshare-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-figshare-data.yaml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:cert@eur.nl"
  - 0 issue "sectigo.com"
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eur.nl
  spf: true
hosts:
- cert_expires: Nov  5 14:30:52 2026 GMT
  host: www.eur.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:47:50 2026 GMT
  host: repub.eur.nl
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 27 05:59:14 2026 GMT
  host: pure.eur.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erasmus University Rotterdam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erasmus University Rotterdam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Erasmus University Rotterdam
provider_slug: erasmus-university-rotterdam
slug: erasmus-university-rotterdam-domain-security
source_filename: erasmus-university-rotterdam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 14:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: repub.eur.nl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 10:47:50 2026 GMT\n  hsts: false\n- host: pure.eur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:59:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: eur.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:cert@eur.nl\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/security/erasmus-university-rotterdam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- OAI-PMH
- Netherlands
---
