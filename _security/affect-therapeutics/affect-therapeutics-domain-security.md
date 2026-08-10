---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: affect.com
  note: marketing/product domain; carries no mail records
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affecttherapeutics.com
  note: corporate mail domain; SPF/DMARC live here, not on affect.com
  spf: true
  spf_record: v=spf1 include:dc-aa8e722993._spfm.affecttherapeutics.com ~all
hosts:
- cert_expires: Oct 29 17:24:11 2026 GMT
  host: www.affect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:48:31 2026 GMT
  host: api.affect.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: Private application backend (nginx on Aptible, CNAME elb-affect-prod-111057.aptible.in). Root returns an HTML "Login Required" page with meta robots=noindex; every contract-discovery path (/openapi.json, /swagger.json, /graphql, /docs, /.well-known/*) returns a genuine 404 verified against a control path. Not a public API — no developer program points at this host.
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:45:46 2026 GMT
  host: www.affecttherapeutics.com
  hsts: false
  https: true
  note: 301 redirects to https://www.affect.com/
  tls_version: TLSv1.3
- host: help.affecttherapeutics.com
  http_status: 200
  https: true
  note: Kustomer-hosted member help center
kind: domain-security
layout: security
method: probed
name: Affect Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affect Therapeutics, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Affect Therapeutics
provider_slug: affect-therapeutics
slug: affect-therapeutics-domain-security
source_filename: affect-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:24:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.affect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:48:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  http_status: 200\n  note: >-\n    Private application backend (nginx on Aptible, CNAME elb-affect-prod-111057.aptible.in).\n    Root returns an HTML \"Login Required\" page with meta robots=noindex; every contract-discovery\n    path (/openapi.json, /swagger.json, /graphql, /docs, /.well-known/*) returns a genuine 404\n    verified against a control path. Not a public API — no developer program points at this host.\n- host: www.affecttherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:45:46 2026 GMT\n  hsts: false\n\
  \  note: 301 redirects to https://www.affect.com/\n- host: help.affecttherapeutics.com\n  https: true\n  http_status: 200\n  note: Kustomer-hosted member help center\ndomains:\n- domain: affect.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  note: marketing/product domain; carries no mail records\n- domain: affecttherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:dc-aa8e722993._spfm.affecttherapeutics.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  note: corporate mail domain; SPF/DMARC live here, not on affect.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affect-therapeutics/refs/heads/main/security/affect-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- Mental Health
- Behavioral Health
- Substance Use Disorder
- Addiction Treatment
- Medicaid
---
