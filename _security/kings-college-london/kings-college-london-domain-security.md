---
api_specs:
- filename: kings-college-london-altmetric-api-openapi.yml
  format: yaml
  label: King's College London altmetric API
  slug: kings-college-london-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-altmetric-api-openapi.yml
- filename: kings-college-london-articles-api-openapi.yml
  format: yaml
  label: King's College London articles API
  slug: kings-college-london-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-articles-api-openapi.yml
- filename: kings-college-london-authors-api-openapi.yml
  format: yaml
  label: King's College London authors API
  slug: kings-college-london-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-authors-api-openapi.yml
- filename: kings-college-london-collections-api-openapi.yml
  format: yaml
  label: King's College London collections API
  slug: kings-college-london-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-collections-api-openapi.yml
- filename: kings-college-london-institutions-api-openapi.yml
  format: yaml
  label: King's College London institutions API
  slug: kings-college-london-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-institutions-api-openapi.yml
- filename: kings-college-london-oauth-api-openapi.yml
  format: yaml
  label: King's College London oauth API
  slug: kings-college-london-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-oauth-api-openapi.yml
- filename: kings-college-london-other-api-openapi.yml
  format: yaml
  label: King's College London other API
  slug: kings-college-london-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-other-api-openapi.yml
- filename: kings-college-london-profiles-api-openapi.yml
  format: yaml
  label: King's College London profiles API
  slug: kings-college-london-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-profiles-api-openapi.yml
- filename: kings-college-london-projects-api-openapi.yml
  format: yaml
  label: King's College London projects API
  slug: kings-college-london-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-projects-api-openapi.yml
- filename: kings-college-london-symplectic-api-openapi.yml
  format: yaml
  label: King's College London symplectic API
  slug: kings-college-london-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-symplectic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kcl.ac.uk
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.kcl.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: kclpure.kcl.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: kcl.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kings College London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for King''s College London, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: King's College London
provider_slug: kings-college-london
slug: kings-college-london-domain-security
source_filename: kings-college-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kcl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kclpure.kcl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: kcl.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kcl.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/security/kings-college-london-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- OAI-PMH
- Library
- United Kingdom
---
